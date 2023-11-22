# Epic Games - Fortnite - Cosmetics - BR - V1 - Images
Retrieve Fortnite player avatar information using this API.

**URL:** `http://api.krowzie.uk/epic/Fortnite/Cosmetics/BR/V1/images/CID`  
**Method:** GET  


## Path Parameters

- `CID`: The cosmetics target id (example: CID_165_ATHENA_COMMANDO_M_DARKVIKING)



## Example
```javascript
const axios = require('axios');

const rq = await axios.get(
  `http://api.krowzie.uk/epic/Fortnite/Cosmetics/BR/V1/images/:CID`,
  {},
  {
    headers: {
      'Content-Type': 'application/json',
      Authorization: 'Bearer TOKEN',
    },
  }
);

console.log("Got imag:", rq.data);
```

## Response

```bash
[
 
  http://api.krowzie.uk/epic/Fortnite/Cosmetics/BR/V1/images/CID_165_ATHENA_COMMANDO_M_DARKVIKING
]
```

##  That gets a large image of the CID

You can use `.png` at the end of the url if you like to


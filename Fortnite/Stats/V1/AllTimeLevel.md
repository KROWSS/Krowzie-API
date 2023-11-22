# Epic Games - Fortnite - Stats - V1 - AllTimeLevel
Retrieve Fortnite player avatar information using this API.

**URL:** `http://api.krowzie.uk/epic/Fortnite/Stats/V1/AllTimeLevel/:accoundId`  
**Method:** GET  
**Auth Required:** Yes

## Path Parameters

- `accountId`: The target account id

## Headers

- `Authorization`: Bearer "Token": The account's token

## Example
```javascript
const axios = require('axios');

const rq = await axios.get(
        `http://api.krowzie.uk/epic/Fortnite/Stats/V1/AllTimeLevel/:accoundId`,
        
        {
          headers: {
            'Content-Type': 'application/json',
            'Authorization': `Bearer ${auth.access_token}`,
          },
        }
      );

console.log("Got info:", rq.data);
```

## Response

```bash
[
 
  startTime: 0,
    endTime: 9223372036854776000,
    stats: { s22_social_bp_level: 10014 },
    accountId: 'Users-Acc-Id'

]
```



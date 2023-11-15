# Epic Games Get Avatar - Fortnite

Retrieve Fortnite player avatar information using this API.

**URL:** `http://api.krowzie.uk/avatar/:accountId`  
**Method:** GET  
**Auth Required:** Yes

## Path Parameters

- `accountId`: The target account id

## Headers

- `Authorization`: Bearer "Token": The account's token

## Example
```javascript
const axios = require('axios');

const rq = await axios.get('http://api.krowzie.uk/avatar/THEACCID', {
  headers: {
    Authorization: 'Bearer TOKEN',
  },
});

console.log(rq.data);
```

## Response

```json
[
  {
    "accountId": "the id of user",
    "namespace": "fortnite",
    "avatarId": "ATHENACHARACTER:CID_165_ATHENA_COMMANDO_M_DARKVIKING"
  }
]
```


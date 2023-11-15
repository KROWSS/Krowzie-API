# Epic Games Get Avatar - Fortnite

Retrieve Fortnite player avatar information using this API.

**URL:** `http://api.krowzie.uk/epic/Fortnite/QueryProfile/easy-athena/:accountId`  
**Method:** GET  
**Auth Required:** Yes

## Path Parameters

- `accountId`: The target account id

## Headers

- `Authorization`: Bearer "Token": The account's token

## Example
```javascript
const axios = require('axios');

const rq = await axios.post(
  `http://api.krowzie.uk/epic/Fortnite/QueryProfile/easy-athena/:accountId`,
  {},
  {
    headers: {
      'Content-Type': 'application/json',
      Authorization: 'Bearer TOKEN',
    },
  }
);

console.log("Got info:", rq.data);
```

## Response

```bash
[
 
  profileRevision: 56897,
  profileId: 'athena',
  profileChangesBaseRevision: 59997,
  profileChanges: [ { changeType: 'fullProfileUpdate', profile: [Object] } ],
  profileCommandRevision: 49030,
  serverTime: '2023-11-15T19:46:11.410Z',
  responseVersion: 1

]
```

##  From There you can see your profile Object!


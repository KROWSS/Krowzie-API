# Epic Games Get Avatar - Fortnite

Retrieve Fortnite player avatar information using this API.

**URL:** `http://api.krowzie.uk/epic/account/accountdetails/:DisplayName`  
**Method:** GET  
**Auth Required:** Yes

## Path Parameters

- `DisplayName`: The target account's DisplayName

## Headers

- `Authorization`: Bearer "Token": The account's token

## Example
```javascript
const rq = await axios.get(
        `http://api.krowzie.uk/epic/account/accountdetails/:DisplayName`,
        {
          headers: {
            'Content-Type': 'application/json',
            Authorization: 'Bearer TOKEN',
          },
        }
      );

console.log(rq.data);
```

## Response

```bash
[
  data {
  id: 'AccountID',
  displayName: 'The DisplayName',
  name: 'Name of requested Account',
  email: 'support@krowzie.uk',
  failedLoginAttempts: 0,
  lastLogin: '2019-06-02T10:41:19.928Z',
  numberOfDisplayNameChanges: 70,
  dateOfBirth: 'D-O-B',
  ageGroup: 'ADULT',
  headless: false,
  country: 'GB',
  lastName: 'LAST NAME',
  phoneNumber: 'NUMBER',
  company: 'KROWZIE',
  preferredLanguage: 'en',
  links: {},
  lastDisplayNameChange: '2023-11-02T12:32:56.761Z',
  canUpdateDisplayName: false,
  canUpdateDisplayNameNext: '2023-11-16T12:32:56.761Z',
  tfaEnabled: true,
  emailVerified: true,
  minorVerified: false,
  minorExpected: false,
  minorStatus: 'NOT_MINOR',
  cabinedMode: false,
  hasHashedEmail: false
}
]
```


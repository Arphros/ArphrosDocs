# User
This is user class, store (almost) everything about user
```ts
    class User {
        public username: string;     // Username
        public id: number            // User Id
        public info: string          // Info about user (e.g. badges)
        public about: string         // User about me (For Supporter)
    }
```


## POST /user
Get user data
Params:
`id` -- User id (Required)
Returns:
`object` -- User data
Examples:
```js
fetch('https://arphros.vercel.app/api/user/user', {
	method: 'POST',
	body: JSON.stringify({ id: '1' })
})
    .then(res => res.json())
    .then((data) => {
        console.log(data)
    })
```
Output:
```js
{
    user: {
        about: "..."
        id: 1
        info: "{\"coins\": 0, ... }"
        username: "Pururut"
    }
}
```
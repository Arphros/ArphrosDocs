## Levels
This is levels class, store everything about levels
```ts
    class Levels {
        public name: string           // The name of the level
        public id: number             // The level ID
        public authorId: number       // Level author ID
        public info: object           // Store info of level
        public verify: boolean        // Is level verify
        public difficulty: string     // Level difficulty
        public time: number           // When was the level created    
    }
```


## POST /getLevel
Get level data
Params:
`id` -- Level id (Required)
Returns:
`object` -- Level data
Examples:
```js
fetch('https://arphros.vercel.app/api/level/getLevel', {
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
    level: {
        name: "Good Taste Good"
        id: 1
        authorId: "1"
        description: "When you want to rick and roll"
        version: 69
        info: "{\"songname\": 'Never gonna give you up', ... }"
        verify: true
        difficulty: 'Hard'
    }
}
```


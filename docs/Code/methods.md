# GetObjectByName(name: string)
Return the object by finding the name of each objects in level.

```lua
local Stones     = GetObjectByName("Stone")
local BlueStones = GetObjectByName("BlueStone")
local Trees      = GetObjectByName("Trees")
```


Returns `Object` class


# GetObjectByID(id: int)
Return the object by finding the first object group of each objects in level.

```lua
local Fish = GetObjectByID(5)
```


Returns `Object` class


# GetObjectsByID(id: int)
Return the array of objects by finding the object group of each objects in level.

```lua
    local GroupObject = GetObjectsByID(3)
    
    for obj in GroupObject do
        ...
    end
```
Returns `array of Object` class


# Object.position 
Get position of the object  
Examples:
```lua
local targetObject = GetObjectByName("MyObject");
local position = targetObject.position
```

Return `Vector` class


# Object.scale
Get scale of the object  
Examples:
```lua
local targetObject = GetObjectByName("MyObject");
local scale = targetObject.scale
```
Return `Vector` class

# Object.rotation
Get rotation of the object  
Examples:
```lua
local targetObject = GetObjectByName("MyObject");
local rotation = targetObject.rotation
```
Return `Vector` class

# Object.Move()
Move the target object.  

Parameters:  
`targetPosition` -- Vector  
`time` -- Float  
`easing` -- EasingType  

Examples:
```lua
local targetObject = GetObjectByName("MyObject");
local targetPosition = Vector(5, 5, 5)
targetObject.Move(targetPostion, 1, "easeInOutQuad")
```
Return `void`


# Object.Scale() 
Scale the target object.

Parameters:  
`targetScale` -- Vector  
`time` -- Float  
`easing` -- EasingType  

Examples:
```lua
local targetObject = GetObjectByName("kulkul object");
local targetScale = Vector(5, 5, 5)
targetObject.Scale(targetScale, 1, "easeOutSine")
```
Return `void`

# Object.Rotate()
Rotate the target object.

Parameters:  
`targetRotation` -- Vector  
`time` -- Float  
`easing` -- EasingType  

Examples:
```lua
local targetObject = GetObjectByName("kulkul object");
local targetRotate = Vector(5,5,5)
targetObject.Rotate(targetRotate,1,"easeOutSine")
```
Return `void`

# Fullscreen() 
Fullscreen the game window.  
Examples:
```lua
if seconds > 10 then
    Fullscreen()
end
```
Return `void`

# Windowed() 
Windowed the game window.  
Examples:
```lua
if seconds < 10 then
    Windowed()
end
```
Return `void`

# MoveWindow() 
Move the game window to specified target
Parameters:
`x` -- Int
`y` -- Int
`time` -- Float
`easing` -- EasingType

Examples
```lua
MoveWindow(300, 175, 1, "easeOutQuart")
```
Return `void`

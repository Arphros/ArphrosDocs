# Object
This object class stores the data about each of objects in level for specify the object name, group, position, rotation and scale
```C#
    public class Obj {
        string name;
        int[]  group;
        Vector position;
        Vector scale;
        Vector rotation;
    }
```

# Vector
The class for store the position, rotation and scale for object.

```C#
    public class Vector {
        float x;
        float y;
        float z;
    }
```
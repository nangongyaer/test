# How to Bulid a Game World
- What does a game world consist of?
- How should we describe these things?
- How are these things organized?

## Dynamic Game Objects
## Static game object
## Environment
- sky 
- vegetation
- terrain
## Other Game Objects
- Air wall
- Trigger Area
## Everything is a Game Object
- Game Object(GO)
## How to Describe a Game Object
- I want a drone
## How Do We Describe a Drone in Reality?
- Shape(property)
- Position(property)
- Move (behavior)
- Capacity of battery(property)
- Etc.
> 几乎所有的物体都可以用property,behavior来描述。
## Game Object
```cpp
class Drone
{
public:
    /* Properties*/
    Vector3 position;
    float health;
    float fuel;
    ...
    /* Behavior*/
    void move();
    void scout();
    ...
};
```
## No Perfect Classification in the Game World!
## Component Base
- Component Composition in the Real World
> 用组件代替继承
## Component of a Drone
```
      --Transform
Drone --Motor
      --Model
      --AI
      --Animation Physics
```


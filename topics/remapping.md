# Remapping
Consider i am writing one library with a node, which subscribes to some topic and processes it, and publishes another topic. 

The one who is using the program, may have different topic name, now he have edit my code and change the name of the topic my code subscribes to?
 
**No**, we have something called remapping. **We don't have to edit the code.**

Consider my node subscribes to the topic `/camera_image` and publishes `/camera_image_improved`

And  want give image from the topic `/kinetic/image` and wants output as `/output`

```xml
<node name='mynode' type="sample_node" pkg="sample_pkg" >
    <remap from="/camera_image" to="/kinetic/image"/>
    <remap from="/camera_image_improved" to="/output"/>
</node>
```
or 

```
rosrun sample_pkg sample_node camera_image:=/kinetic/image camera_image_improved:=/output
```

## Resources
- http://wiki.ros.org/roslaunch/XML/remap
- http://wiki.ros.org/Remapping%20Arguments
- http://wiki.ros.org/Names

## Ask yourself
- [ ] For topics okay, if I want to remap parameters, is it possible to do?
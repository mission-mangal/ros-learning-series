- [ros-learning-series](#ros-learning-series)
  - [Topics](./topics/topics.md)
    - [Namespace](./topics/namespace.md)
    - [Remapping](./topics/remapping.md)
  - [Nodes](./nodes/README.md)
    - [Publisher](./nodes/publisher.md)
    - [Subscriber](./nodes/subscriber.md)
    - [Service](./nodes/rosservice.md)
    - [Client](./nodes/client.md)
    - [Action Server](./nodes/action_server.md)
    - [Action Client](./nodes/action_client.md)


> Each .md file contains practice question and question to think.

## Instructions
Fork this repository to your account
```
git clone https://github.com/<username>/<repository_name>
cd <repository_name>
```

Create one ros package named *ros_learning_series*
```
mkdir -p ros_learning_series/src
catkin create pkg ros_learning_series std_msgs std_srvs roscpp rospy actionlib
```
Inside write you codes with the name provided in each qn.
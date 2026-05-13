Affordance
    graspable
    placeable
    supportable

动作原语
    navigate: Collision-free trajectory of the entire robot to a location.
    pick: Composition of 1) a trajectory to a pre-grasp 6D_pose above the object to pick, 2) a  line trajectory in Cartesian space down towards the object, interrupted when there is contact, 3) a closing action, 4) a first retracting trajectory following a line upwards, and 5) a second retracting trajectory to reach the untucked joint configuration.
    place: Composition of 1) a trajectory to a pre-place 6D_pose above the object to place the  grasped object on, 2) an opening action, 3) a second retracting trajectory to reach the untucked joint configuration.

谓词
    grasped
    on
对物体资产的要求
原点位于地面中心，而不是物体几何中心
遵循z up
x为front方向

如果是机器人
    +z朝上
    +x机器人朝前方向
如果是笔
    +x 笔尖朝前方向
如果是二维码
    相对复杂一些，二维码是贴在一个平面上
如果是扫码枪
    +x垂直于扫码的镜面


# From Omniverse SimReady Definition
All 3D assets need to be built to real-world scale
Orientation for an exported 3D model should always be Z-up and it should always be placed at the origin
Required unit scale for export is always set to meters
The 3D asset must face Front in the “front” viewport of the chosen DCC or CAD app
When working in a DCC app, create assets with optimal geometry for curvature without wasting polygons
Name all elements within your asset cleanly so they are easily identifiable (no Box01 or pSphere27)
Pivot points must be placed and aligned so the asset “sits” properly with respect to the ground plane


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

识别出来的
    颜色会有变化
    方位会有变化
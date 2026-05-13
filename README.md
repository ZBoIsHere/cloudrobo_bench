# 任务场景格式定义

scene_cfg.json解释

动作原语
    NAVIGATE: collision-free paths of the entire robot to navigate to a location
    PICK: pre_place 6D pose; a line trajetory toward object; a close action; retracting line trajectory; to joints
    PLACE: pre_palce 6D pose; opeing aciton; retracting trajectory
    ROTATE:
    HANDOVER：左右手交换
    INSERT (插入)：将一个物体精准放入另一个物体的孔洞或槽位（如航插插拔）
    OPEN (打开)：沿铰接路径（转动或平移）改变物体（如门、抽屉）的开启度
    CLOSE (关闭)：将开启状态的铰接物体恢复至闭合状态
    PULL：拉，比如把抽屉拉开
    PUSH：推，比如把箱子推走
    TURN：旋拧，比如旋转煤气灶旋钮
    ALIGN：使得两个物体能够对其，比如扫码器能够对准二维码


// 物体可能是多种；执行臂也可能是多种
// 左右臂并行pick，可能是做，也可能是右
// 如果有多个目标物体怎么办


基础任务
    PICK_AND_PLACE
    STACK
    HANG: 悬挂，把杯子挂到衣架上

谓词列表
    GRASPED
    NEAR
    AT
    ON
    IN

    
需要对desk进行标注，也就是他的支撑平面是什么
# OptimusPrime_risk_dataset
this is a dataset of risk in Auto vehicles

这是V1.1版本的数据集
里面是Carla中采集的GCN训练数据集


# 解释


node_dict = {
    "ego": 0, "person": 1, "bicycle": 2, "car": 3, "motorbike": 4, "aeroplane": 5, "bus": 6, "train": 7, "truck": 8,
    "boat": 9, "traffic light": 10, "fire hydrant": 11, "stop sign": 12, "parking meter": 13, "bench": 14, "bird": 15,
    "cat": 16, "dog": 17, "horse": 18, "sheep": 19, "cow": 20, "elephant": 21, "bear": 22, "zebra": 23, "giraffe": 24,
    "backpack": 25, "umbrella": 26, "handbag": 27, "tie": 28, "suitcase": 29, "frisbee": 30, "skis": 31, "snowboard": 32,
    "sports ball": 33, "kite": 34, "baseball bat": 35, "baseball glove": 36, "skateboard": 37, "surfboard": 38,
    "tennis racket": 39, "bottle": 40, "wine glass": 41, "cup": 42, "fork": 43, "knife": 44, "spoon": 45, "bowl": 46,
    "banana": 47, "apple": 48, "sandwich": 49, "orange": 50, "broccoli": 51, "carrot": 52, "hot dog": 53, "pizza": 54,
    "donut": 55, "cake": 56, "chair": 57, "sofa": 58, "pottedplant": 59, "bed": 60, "diningtable": 61, "toilet": 62,
    "tvmonitor": 63, "laptop": 64, "mouse": 65, "remote": 66, "keyboard": 67, "cell phone": 68, "microwave": 69,
    "oven": 70, "toaster": 71, "sink": 72, "refrigerator": 73, "book": 74, "clock": 75, "vase": 76, "scissors": 77,
    "teddy bear": 78, "hair drier": 79, "toothbrush": 80,

    "Invaded-lane":81, "In-lane":82, "Potential—left":83,"Potential—right":84, "Left-lane":85, "Right-lane":86, "Safe-zone":87,
    "On-ground":88, "In-air":89, "Stationary":90, "kinetic":91,
    "Straight":92, "Intersection":93
}

edge_attr = {
    "visible-Top-Left": 0, "very_far-Top-Left": 1,  "far-Top-Left": 2,  "near-Top-Left": 3, "very_near-Top-Left": 4,
    "close-Top-Left": 5,"extremely_close-Top-Left": 6,   "dangerous_distance-Top-Left": 7,
    "visible-Top-Right": 8, "very_far-Top-Right": 9,  "far-Top-Right": 10,  "near-Top-Right": 11, "very_near-Top-Right": 12,
    "close-Top-Right": 13,"extremely_close-Top-Right": 14,   "dangerous_distance-Top-Right": 15,
    "visible-Top-Middle": 16, "very_far-Top-Middle": 17,  "far-Top-Middle": 18,  "near-Top-Middle": 19, "very_near-Top-Middle": 20,
    "close-Top-Middle": 21,"extremely_close-Top-Middle": 22,   "dangerous_distance-Top-Middle": 23
}




******************示例如下：

new_node_feature:
1.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 1.000000 0.000000 0.000000 1.000000 0.000000 1.000000
0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 1.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 0.000000 1.000000 0.000000 0.000000 0.000000 0.000000 1.000000 0.000000 1.000000 0.000000 0.000000 1.000000

new_edge_index:
0 1
0 2


new_edge_attr:
19.000000
8.000000


dangerous:    分别代表安全、碰撞、追尾、鬼探头
0.800000
0.050000
0.100000
0.050000






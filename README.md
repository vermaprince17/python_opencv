To compare the output for openCV and TF calls,

1. cd to samples/dnn/
2. from the above directory,
   python -m dnn_model_runner.dnn_conversion.tf.classification.py_to_py_mobilenet

and for visualization,

python -m dnn_model_runner.dnn_conversion.tf.classification.py_to_py_cls --model_name mobilenet --test True --default_img_preprocess True --evaluate False

3. python object_detection.py --model ../../ssd_mobilenet_v1_coco_2017_11_17/frozen_inference_graph.pb --config ../../ssd_mobilenet_v1_coco_2017_11_17/ssd_mobilenet_v1_coco_2017_11_17.pbtxt  --input ../../pexels_double_decker_bus.jpg --width 300 --height 300 --classes ../../object_detection_classes_coco.txt

3. Make sure you have TF 2.4.0 with MacOS build.

# yolo_to_matlab_dataset
Converting YOLO Dataset to MATLAB for Use in Image Labeler

Overview:
This guide will walk you through the process of converting a YOLO dataset to MATLAB format, allowing you to use it efficiently in the Image Labeler app. The provided code is designed for a dataset with two objects, but it can be easily adapted for datasets with more classes by making a few simple modifications.

Steps:

edit files with your classes names

Organize Your Dataset:
Place the images and their corresponding labels in a single folder. Ensure that each image has a corresponding label file in the YOLO format (e.g., .txt files with bounding box coordinates).

Create the Dataset Table:
Utilize the create_table.mlx MATLAB script to create a dataset table. This table will help manage the information associated with your images and annotations.

Load Images into Image Labeler:
Open the Image Labeler app and load your dataset's images into the app for annotation.

Convert Labels to Ground Truth:
Run the convert_table_to_ground_truth.mlx MATLAB script once for each class in your dataset. This script converts the YOLO format labels to ground truth format for the Image Labeler app.

Load Labels for Each Class:
After running the conversion script for each class, load the generated ground truth labels from the MATLAB workspace into the Image Labeler app.

With these steps, you'll be able to efficiently convert your YOLO dataset into a format compatible with the Image Labeler app in MATLAB. Enjoy annotating and working with your custom dataset for various computer vision tasks!

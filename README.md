# Deep Learning - Lab 4 – YOLO Object Detection

1. Download the `yolo_v2.h5` weights file from the Google Drive link below. It contains the YOLO version 2 pre-trained model weights. Copy the downloaded file to the `model_data` directory.
   - **Link:** [Google Drive](https://drive.google.com/drive/folders/1ogvfqQsLADkVLWt64m-wABDfszHaE8EV?usp=sharing)

2. Zip all folders and files in `lab5.zip` except `lab5_labsheet.docx` and `Autonomous_driving_application_car_detection.ipynb`, and upload the zip file to a Google Drive folder.

3. Upload the Jupyter notebook (`Autonomous_driving_application_car_detection.ipynb`) to the Google Colab root directory. </br> ![image](https://github.com/user-attachments/assets/fd77cd15-5a1c-401c-bd33-362f48b3efdd)
4. In the uploaded notebook, change the path in the second cell to the path of the zip file (created and uploaded in Step 2) and run the first two cells.Root directory should look similar to the below image after this. 

5. Go through the `Autonomous_driving_application_car_detection.ipynb` notebook and try to understand the code.
6. Run the notebook. Make sure to change the `dest_folder` path in the final cell before running it.At the end, you should see:
     - Result of the car detection demo (`test.jpg`).
     - Results of the random images (`giraffe_resized.jpg` and `DSC_1643_resized.jpg`).
     - Results of all images in the autonomous driving dataset (`0100.jpg` to `0120.jpg`) saved to the `out` directory.
     - A zip file containing all the above images in the Colab root as well as in your Google Drive.

7. In the below-given cell, the shape of `boxes.eval()` is `(17834)`. Why are there 1783 boxes? Explain the reason for it. What is the maximum number and minimum number you can get for that? Write these answers in a word file.
     - Change the values like `mean` and `stddev` in lines 2 and 4, as well as the `threshold` value in line 5, and observe the different values you get for `boxes.eval().shape` </br></br> ![image](https://github.com/user-attachments/assets/61d20675-3902-49ac-9f8f-1d18b2d6d823)
8. `yolo_anchors.txt` contains 10 values. They can be considered as the height and width of 5 anchor boxes. What is the advantage of using such anchor boxes? What was the method used to determine the sizes of these anchor boxes? Give the answers to these questions in the Word file.

9. Upload a new traffic image to the `images` directory and edit the code as needed to detect vehicles in that image.

10. Download the output `images zip` file from Google Drive and observe the bounding boxes in the autonomous driving dataset (i.e., 21 images from `0100.jpg` to `0120.jpg`). Select 2 images from these 21 images and,
    - Write what you observe regarding correctly detected objects, incorrectly detected objects, undetected objects and incorrect bounding boxes in the word file.
    - Include these `output 2` images as well as the original 2 images in the word file. 

    Include these 2 output images as well as the original 2 images in the Word file.

12. Adjusting parameters like `max_boxes`, `score_threshold`, and `iou_threshold` of the `yolo_eval` function can potentially address the limitations you noticed in Step 10.

    - Change the `max_boxes` [integer value] to a different value but use the original values for the other 2 variables. Rerun the required cells to get the output images for the autonomous driving dataset. Observe if this results in improvement compared to Step 10 for the same two images. If there are any improvements, write them in the Word file. Include the new 2 output images in the Word file.
    - Change the `score_threshold` [value between 0-1] to a different value but use the original values for the other 2 variables. Rerun the required cells to get the output images for the autonomous driving dataset. Observe if this results in improvement compared to Step 10 for the same two images. If there are any improvements, write them in the Word file. Include the new 2 output images in the Word file.
    - Change the `iou_threshold` [value between 0-1] to a different value but use the original values for the other 2 variables. Rerun the required cells to get the output images for the autonomous driving dataset. Observe if this results in improvement compared to Step 10 for the same two images. If there are any improvements, write them in the Word file. Include the new 2 output images in the Word file.

## Submission

- Download the final modified `Autonomous_driving_application_car_detection.ipynb` notebook. Add this notebook, the new image used in Step 9, and the Word file to a new zip file.
- Upload this zip file to the course web submission link. The file name should be your registration number.
  
___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>



# DeepLearning – Labsheet 3

1. **Upload** `Face_Recognition_for_the_Happy_House_v2.ipynb` to Google Colab.
2. **Upload** the `fr_utils.py` and `inception_blocks_v2.py` files to the root (`/content`) directory of the VM.
3. **Create** a folder called `images` in the root (`/content`) directory in the VM and **upload** the images in the `images` directory to the `images` directory in the VM.
4. **Download** the `weights.zip` file from this [Google Drive link](https://drive.google.com/drive/folders/1IExxks0GFQCCj6z8Wh0lWxW7NRndclZS?usp=sharing) and **upload** the `weights.zip` file to the VM root (`/content`) directory.
   
5. **Run** the Jupyter notebook.
6. **Upload** an image of yourself or another individual to the `images` directory and **encode and add it to the database** mentioned in the notebook.
7. **Replace** the image of Younes with another image of the same individual you chose in step 6 to perform both **face verification and face recognition**.
   - Make sure these new images have the required height and width. Use the `tensorflow.image.resize()` method if needed.
8. **Add** the two new images and **screenshots of outputs** from both face verification and face recognition of step 7 to a Word file.
   - Specifically, ensure the screenshot of `output[2]` from the face recognition task is included.
   - Note: `output[2]` is a dictionary containing the L2 distance between the target image encoding and the database embeddings of other images.

## NOTE:
-The `weights.zip` file is not added to the repository. Please download it using the [provided drive link](https://drive.google.com/drive/folders/1IExxks0GFQCCj6z8Wh0lWxW7NRndclZS?usp=sharing)
-The images of `Indudini Thennakoon` and `Madhusha Silva` have been added to the images folder.
-The answer sheet, including screenshots for Task 6 to Task 8, is in the `IT21170966_labsheet3_Answer.docx` word document.
-The modified notebook is available in the repository.



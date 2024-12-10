# Flipkart_Grid_Robotics-Level 2
This project aims to develop the smart vision quality checking system using the Artificial Intelligence. I use the Qwen2-VL-2B model for text recognition &amp; decision making from the images.
![image](https://github.com/user-attachments/assets/33de1a34-73b3-4b45-a5b8-2ba0e05f3eb5)
# Use the google collaboratory for running of the project as it requires good GPU and the disk storage.

step 1) Open the Flipkart_Grid_Model_PhaseII.ipynb

step 2) Download the Required Dependencies

step 3) Import the Models and Libraries

step 4) Run the cell containing all Functions
  - File Preprocessing
  - take_photo(): To capture the photo from webcam in real time
  - process_image(): To process the captures image by the Qwen2-VL-2B Model and generate the python dictionary containing all attributes
  - Normalize the Expiry Date
  - append_to_excel(): Add the data in product_analysis.xlsx file

Tries to Fine Tune it using the LLaMA-Factory but not significant difference from pretrained model...maybe due to limited data

The model I used : https://huggingface.co/Qwen/Qwen2-VL-2B-Instruct

Future Scope:
- Fine Tuning it to train model for the Smart_Vision_Quality_Testing only
- Deploy on NIM/GCP/AWS/Azure any cloud to remove dependency from Collab
- Use DroidCam or IPWebCam feature as its possible after getting it deployed on Hybrid Model to get portability.
- Frontend for better user experience



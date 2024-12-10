# Flipkart_Grid_Robotics-Level 2
This project aims to develop the smart vision quality checking system using the Artificial Intelligence. I use the Qwen2-VL-2B model for text recognition &amp; decision making from the images.
The model I used : https://huggingface.co/Qwen/Qwen2-VL-2B-Instruct
![image](https://github.com/user-attachments/assets/33de1a34-73b3-4b45-a5b8-2ba0e05f3eb5)

**Q: Why should I use the Qwen/Qwen2VL-2B-Instruct model instead of other ML models, DL models, or LLMs?**

**A:** The Qwen/Qwen2VL-2B-Instruct model is particularly effective for instruction-following tasks and excels in both NLP and visual understanding. Compared to traditional ML and DL models, it is optimized for handling multimodal input, such as combining image and text for product analysis. It offers enhanced accuracy in tasks involving complex context and structured data extraction, which is essential for projects like yours.

- **Traditional ML Models:** Many ML models (e.g., decision trees, random forests, SVM) perform well on structured data but struggle with unstructured data like images or text. They also typically require more feature engineering and domain-specific knowledge, making them less flexible for tasks like multimodal analysis.
  
- **Deep Learning (DL) Models:** While DL models (e.g., CNNs, RNNs, and transformers) can handle complex tasks, they may require large amounts of labeled data, significant computational resources, and fine-tuning to perform well. Models like CNNs are excellent for image tasks but typically lack the instruction-following capability, making them less ideal for tasks that combine both vision and language.

- **LLMs:**  
While LLMs like GPT-3 or GPT-4 are powerful in NLP tasks, they often struggle with visual inputs unless specifically adapted for multimodal tasks (e.g., CLIP, BLIP). They also can be less efficient in handling real-time data extraction and structured information from images, making them less suitable for precise tasks like product analysis when a high degree of accuracy is needed across multiple modalities.

In summary, the Qwen/Qwen2VL-2B-Instruct model is specifically optimized for multimodal tasks, offering better performance and efficiency for your use case compared to traditional ML, DL models, and general-purpose LLMs.

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
step 5) Run the last cell containing main peice of code with user run for each product
Tries to Fine Tune it using the LLaMA-Factory but not significant difference from pretrained model...maybe due to limited data

Future Scope:
- Fine Tuning it to train model for the Smart_Vision_Quality_Testing only
- Deploy on NIM/GCP/AWS/Azure any cloud to remove dependency from Collab
- Use DroidCam or IPWebCam feature as its possible after getting it deployed on Hybrid Model to get portability.
- Frontend for better user experience



# Text-Extraction-from-Image-Dataset:  
* Build a Computer Vision project to detect and recognize text from Images. 
* TextOCR dataset is used which provides ~1M high quality word annotations on TextVQA1000.
* Three build-in libraries i.e. pytesseract, easyocr, keras_ocr for optical character recognition are compared to find the most accurate one.

## Data Collection
Kaggle [Dataset](https://www.kaggle.com/datasets/robikscube/textocr-text-extraction-from-images-dataset?select=annot.csv) is being loaded and then fully analyzed. 
The dataset contains six columns:
* id (annotation id)
* image_id (image id)
* bbox (bounding box)  
* utf8_string (text annotation)
* points (point location of text)
* area (area of text in image)

## Model Comparision
We need to build a model to recognize the text not in ideal condition from different images. Three build-in python OCR models are compared both in terms of accuracy and how long they take to extract text from images with each other. These three models are as follow:
* pytesseract
* easyocr  
* keras_ocr

pytesseract is not able to work efficiently with our dataset. Mean while both easyocr and keras_ocr works fine. When first 25 examples are manually analyzed for accuracy easy ocr was giving better results and it was also not splitting the senences in seperate words.


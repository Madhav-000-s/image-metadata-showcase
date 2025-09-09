## 🏃‍♀️ How to Use

### 1. Open in Colab
Click the badge below to launch the notebook in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Madhav-000-s/image-metadata-showcase/blob/main/notebook/Image_Metadata_Analysis_final.ipynb)

---

### 2. Run the Notebook

1. **Setup** → Installs required libraries  
2. **Upload Images** → Upload your own images from your computer  
3. **Fetch from GitHub** → Optionally, pull all images from this repo’s `images/` folder  
4. **Helper Functions** → Defines metadata + OCR utilities  
5. **Process & Display** → Runs extraction and displays results inline  

---

## 🧰 Dependencies

The notebook installs all dependencies automatically in Colab, including:

- [Pillow](https://python-pillow.org/) (image processing)  
- [ExifRead](https://pypi.org/project/ExifRead/) (metadata parsing)  
- [OpenCV](https://opencv.org/) (image handling)  
- [pytesseract](https://pypi.org/project/pytesseract/) (OCR)  
- [langdetect](https://pypi.org/project/langdetect/) (language detection)  
- [matplotlib](https://matplotlib.org/) (visualization)  
- [pandas](https://pandas.pydata.org/) (summary tables)  

---

## 📊 Example Output

For each image, you’ll see:

- **Preview of the image**
- **OCR snippet** (first ~240 characters of text)
- **Language detected**
- **GPS coordinates** (if available)
- **Key EXIF fields**
- **Summary table** at the end  

---

## 📜 License

This project is open-sourced under the **MIT License**.

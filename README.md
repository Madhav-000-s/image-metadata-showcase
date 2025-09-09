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

## 📑 What Can Be Extracted from Image Metadata?

Image files often carry **hidden metadata** (EXIF, IPTC, XMP) that records details about how, when, and where they were created or edited. Here are the key categories:

---

### 📸 Camera & Device Information
- **Make / Model** → Device brand & model (*Canon EOS 80D, iPhone 14*).  
- **Lens Info** → Lens model, focal length, zoom.  
- **Serial Numbers** (sometimes) → Unique identifiers for the camera or lens.  

👉 *Tells you which device captured the image.*

---

### 🕒 Date & Time
- **DateTimeOriginal** → When the photo was taken.  
- **CreateDate / ModifyDate** → When the file was created or last edited.  
- **SubSecTimeOriginal** → Fractions of seconds for precision.  

👉 *Helps establish the capture timeline.*

---

### 🌍 Location (GPS)
- **Latitude / Longitude** → Exact coordinates.  
- **Altitude** → Height above sea level.  
- **ImgDirection** → Compass direction of capture.  
- **GPSDate / GPSTimeStamp** → Time of the GPS fix.  

👉 *Allows geolocation of the image.*

---

### ⚙️ Camera Settings
- **ExposureTime** → Shutter speed (`1/200 sec`).  
- **FNumber** → Aperture (`f/2.8`).  
- **ISO** → Sensitivity setting (e.g., `ISO 400`).  
- **FocalLength** → Zoom level (`50mm`).  
- **Flash** → Whether flash was fired.  
- **MeteringMode / WhiteBalance / SceneType** → Exposure & lighting settings.  
- **Sharpness / Contrast / Saturation** → In-camera processing hints.  

👉 *Reveals the conditions of capture.*

---

### 🖼️ Image Characteristics
- **Orientation** → Portrait or landscape.  
- **ImageWidth / ImageHeight** → Resolution in pixels.  
- **ColorSpace** → e.g., `sRGB`, `AdobeRGB`.  
- **Compression / BitsPerSample** → Encoding details.  

👉 *Useful for proper display and checking edits.*

---

### 🧭 Software & Editing
- **Software** → App that saved/edited the file (*Photoshop, WhatsApp*).  
- **CustomRendered / DigitalZoomRatio** → Processing applied.  
- **ModifiedDate** → Evidence of editing after capture.  

👉 *Indicates post-processing or sharing apps used.*

---

### 🧾 IPTC & XMP Metadata (if present)
- **Title / Caption / Keywords** → Descriptions for search & cataloging.  
- **Copyright / Author** → Ownership & rights.  
- **Contact Info** → Photographer details.  
- **Usage Rights** → License information.  

👉 *Important for digital rights management.*

---

### ⚠️ Caveats
- Not all images carry metadata (e.g., screenshots, social media exports).  
- Metadata can be stripped (for privacy) or altered (to spoof origins).  
- GPS/location data is particularly sensitive for privacy.  

---

### ✅ Summary
From image metadata, you can often determine:  
- **Who/what** → Device brand/model, author.  
- **When** → Exact capture and edit times.  
- **Where** → GPS coordinates.  
- **How** → Camera settings like exposure, ISO, flash.  
- **What happened later** → Whether the file was edited or shared.  


## 📜 License

This project is open-sourced under the **MIT License**.



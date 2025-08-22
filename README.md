# 🚗 Parking Space Detection System  

This project is a **computer vision–based parking lot monitoring system** built using **Python, OpenCV, and CVZone**.  
It detects **free and occupied parking spaces** in real-time from a parking lot video feed.  

---

## ✨ Features  
- 🔍 Detects **free and occupied parking spots** using image processing  
- 📹 Works with both **images and video streams**  
- 🟢 Marks available spots in **green**, occupied ones in **red**  
- 📊 Displays **count of available spaces** in the frame  
- 🔄 Can loop video like a live CCTV feed  
- ⚡ Lightweight (no deep learning required)  

---

## 🛠 Tech Stack  
- Python 3.x  
- OpenCV (image processing)  
- CVZone (easy visualization utilities)  
- Numpy  

---

## 📷 Working  
1. Load parking lot video footage  
2. Preprocess each frame (grayscale, blur, threshold, dilation)  
3. Crop regions of interest (parking slots from a saved `CarParkPos` file)  
4. Count non-zero pixels in each slot → decide **occupied/free**  
5. Overlay bounding boxes and free slot counter on the video  

---

## 📊 Example Output  
- 🟢 Free slots are shown in **green**  
- 🔴 Occupied slots are shown in **red**  
- 🧮 The total number of free slots is displayed at the top  

---

## 🚀 Installation  

Clone the repo and install dependencies:  

```bash
git clone https://github.com/manvitha-konki/parking_space_counter.git
cd parking_space_counter
pip install -r requirements.txt

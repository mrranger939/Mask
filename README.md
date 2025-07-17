

##  Face Mask Detection with Live Camera Feed

This project is a **real-time face mask detection system** using a webcam. It uses **EfficientNet** as the base model (transfer learning) and OpenCV's **Haar Cascade** for face detection. The model predicts whether a person is **wearing a mask** or **not wearing a mask**, and displays it on the video feed.

---
### 🖼️ Screenshots

<p float="left">
  <img src="https://github.com/user-attachments/assets/bdc8399a-d314-4c0b-ba25-50c29411ba86" width="45%" />
  <img src="https://github.com/user-attachments/assets/11282c76-065f-4efd-ace0-f17623e609cd" width="45%" />
</p>


---

### 📁 Folder Structure

```
.
├── FinalmaskCameraDetect.ipynb     # Main notebook to run live detection
├── my_efficient_model.h5           # Trained EfficientNet model (binary mask classifier)
├── haarcascade_frontalface_default.xml  # Haar Cascade for face detection
├── requirements.txt                # Dependencies
├── README.md
```

---

### 🚀 How to Run

#### ⚙️ 1. Clone the Repository

```bash
git clone https://github.com/mrranger939/Mask.git
cd Mask
```

#### 📦 2. Install Dependencies

You can install everything using `pip`:

```bash
pip install -r requirements.txt
```

Alternatively, if you're running in **Google Colab**, no need to install anything manually. Just upload files and run the cells.

#### 🧠 3. Run the Model with Live Webcam

Simply open and run the notebook:

```bash
FinalmaskCameraDetect.ipynb
```

Make sure the following files are in the same directory:

* `my_efficient_model.h5`
* `haarcascade_frontalface_default.xml`

---

### 📌 Key Features

* Real-time webcam integration using OpenCV.
* Binary classification: `Masked` ✅ or `No Mask` ❌.
* Built using TensorFlow and EfficientNetB0 for speed and efficiency.
* Haar Cascade used for detecting faces before classification.
* Live label drawing on the video feed using OpenCV.

---

### 🧪 Sample Output

On the webcam feed, you'll see a bounding box on each detected face along with a label:

* 🟩 Green box and **Masked** label if mask is detected.
* 🟥 Red box and **No Mask** label if no mask is detected.


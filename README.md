# 👁️ Computer Vision Portfolio – Sadia Saeed

**ITAI 1378 – Computer Vision · Artificial Intelligence program**

This portfolio collects my hands-on work in computer vision. It starts with how a computer stores an image as numbers, then moves through classic machine learning, neural networks and CNNs, to object detection, segmentation, and Vision Language Models that can answer questions about images. Every lab notebook was run in Google Colab and keeps its real outputs.

---

## 📚 Labs
| Lab | Topic | Tools | Key result |
|---|---|---|---|
| [**Lab 02**](Lab02-Image-Processing-Fundamentals/) | Image processing fundamentals: pixels, channels, filters, histograms, transforms | OpenCV, Pillow, NumPy | Built blur, edge, and sharpen filters and 4 artistic effects from basic operations |
| [**Lab 03**](Lab03-SVM-Image-Classification/) | Image classification with an SVM (cat, dog, ship) | scikit-learn, CIFAR-10 | **54.7%** accuracy on 3,000 test images (ships easiest, cats vs. dogs hardest) |
| [**Lab 04**](Lab04-Chihuahua-or-Muffin-Neural-Network/) | Chihuahua or muffin? A neural network | PyTorch | Raised validation accuracy from **56.7% → 90%** by switching to Adam and bigger images |
| [**Lab 05**](Lab05-Chihuahua-or-Muffin-CNN/) | Chihuahua or muffin? A CNN | PyTorch | **93.3%** baseline, up to **96.7%** (100% at peak) with longer training |
| [**Lab 06**](Lab06-Object-Detection-and-Segmentation/) | Object detection and segmentation | YOLO11, YOLO11-seg, SAM 2 | Detected 5 objects (bus 94%); showed the confidence-threshold trade-off (6 → 5 → 4 detections) |
| [**Lab 08**](Lab08-Vision-Transformers-and-VLMs/) | Vision Transformers and Vision Language Models | Hugging Face, SmolVLM-500M | One model for classifying, counting, describing, and reading charts; tested for hallucinations with ground truth |

## 🐾 Final project: PetGuard AI
A computer-vision system that detects pets with YOLO and checks whether they enter a restricted area. The idea started in Lab 06.
➡️ **Repository:** [ITAI1378-ComputerVision-PetGuard-AI](https://github.com/sadia62668/ITAI1378-ComputerVision-PetGuard-AI)

---

## ✨ Highlights
**From a basic network to a CNN (Labs 04 → 05).** The same 120 training images, but convolutions lift validation accuracy from 56.7% to over 93%.
![CNN validation accuracy per epoch](images/highlight_cnn_accuracy.png)

**Detection confidence threshold (Lab 06).** Lower thresholds find more but make mistakes, and higher thresholds are safer but miss objects.
![YOLO11 at three confidence thresholds](images/highlight_yolo_thresholds.png)

**Creative image-processing pipeline (Lab 02).** Effects built only from basic point, filter, and color operations.
![Artistic effects](images/highlight_artistic_effects.png)

---

## 🛠️ Skills practiced
- **Image fundamentals:** pixels as matrices, color channels, grayscale, histograms, convolution kernels, geometric transforms
- **Classic ML:** feature preparation (grayscale, normalization, flattening), SVM, precision/recall/F1
- **Deep learning:** fully connected networks and CNNs in PyTorch, optimizers (SGD vs. Adam), learning rate, epochs, data augmentation, overfitting
- **Detection and segmentation:** YOLO11, YOLO11-seg, SAM 2, confidence thresholds, NMS, IoU
- **Vision Language Models:** ViT patches, prompting for many tasks, alt text, chart reading, hallucination testing, deployment audits

## 📁 Repository structure
```
ITAI1378-ComputerVision-Portfolio/
├── README.md                          ← this page
├── images/                            ← highlight pictures
├── Lab02-Image-Processing-Fundamentals/
├── Lab03-SVM-Image-Classification/
├── Lab04-Chihuahua-or-Muffin-Neural-Network/
├── Lab05-Chihuahua-or-Muffin-CNN/
├── Lab06-Object-Detection-and-Segmentation/
└── Lab08-Vision-Transformers-and-VLMs/
     (each lab folder: README.md + notebook + images/)
```

## ▶️ How to open a lab
Click a lab folder, then click the `.ipynb` file. GitHub shows it with all outputs. To run it yourself, open it in Google Colab (**File → Open notebook → GitHub** → paste this repo's link).

## 🙏 Credits
Lab notebooks and instructions were provided by the ITAI 1378 course. Labs 04–05 are based on the [Chihuahua vs. Muffin workshop](https://github.com/patitimoner/workshop-chihuahua-vs-muffin). The experiments, runs, and written answers are my own. AI assistance (Claude) was used to organize this portfolio and draft the README files.

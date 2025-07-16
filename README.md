3D Tumor Segmentation from PET/CT Scans

This project uses deep learning to automatically detect and segment tumors from 3D PET and CT medical scans.

##  What It Does

We built a 3D U-Net model that takes in paired PET and CT scans and predicts a mask showing the location of soft-tissue sarcomas (tumors). The model learns to recognize tumors by training on real patient data with labeled tumor regions.

##  How It Works

- We use a public dataset from the TCIA Soft Tissue Sarcoma study, preprocessed as `.h5` files
- Each patient has a CT scan, a PET scan, and a tumor mask (all 3D)
- The scans are resized and normalized for training
- A 3D U-Net model is trained using Dice loss to learn from these examples
- Once trained, the model can predict tumors on new patients

##  Why It Matters

Detecting tumors in medical scans is time-consuming and hard. This model helps automate that process, making it faster for doctors to find and analyze tumors. It's also a good starting point for more advanced medical AI tools.

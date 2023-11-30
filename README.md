# MicroGlam✨: Microscopic Skin Image Dataset with Cosmetics
##### Toby Chong, Alina Chadwick, I-Chao Shen, Haoran Xie, Takeo Igarashi
![image](https://github.com/tobyclh/MicroGlam/assets/12501995/8d9dcc93-5b6f-4b55-a970-85be298f9337)

MicroGlam is a dataset of skin patch images from 45 patches (5 skin patches each from 9 participants) of size 8mm $^*$ 8mm under three cosmetic products (i.e., foundation, blusher, and highlighter). 


## Download
[Kaggle](https://www.kaggle.com/datasets/tobyclh/microglam)


## Dataset Content
Images are encoded to HEIF (.heic) to minimize storage requirement.
We recommend directly reading the image as is using library such as [pyheif](https://pypi.org/project/pyheif/).  

### Folder/Filename Convension
After uncompressing the zip, you will find *patch folders* named `S{}_P{}_{product_name}_{handiness}`.  
- `S` stands for subject number, i.e., all `S1` folders come from the same person;
- `P` stands for patch number, i.e., all `S1_P1` folders come from the exact same skin patch;
- `product_name` refers to the product applied onto the skin patch, and
- `handiness` refers to which hand the patch comes from.

In each of the *patch folders*, we have subfolders `1~8`, the number refers to the number of LED light that is lit during the capture.  
All images are named `calibration_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}_{}.heic`, 
Each of the 3 digit numbers refer to the intensity of the LED light (0~200). 
The lighting condition are randomized amoung subjects, but consistent for all patches for the same subject across all patches. 
The relative position of the LED light with regard to the camera is fixed.  

## License
This data is free to use for non-commercial academic research. 


## Contact
For any question please feel free to open an issue and for commercial enquiry please contact our lab at tobyclh@g.ecc.u-tokyo.ac.jp

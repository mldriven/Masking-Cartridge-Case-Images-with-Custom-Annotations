## Masking-Cartridge-Case-Images-with-Custom-Annotations

The forensic laboratory uses a 3D microscope to capture images of fired ammunition components, specifically cartridge cases. These acquired images are then sorted by software for comparison purposes to learn if the cartridges in question came from the same or different firearms, which is information of great value to police investigations. Masking/colouring is a preparatory function, currently performed manually, which assists the software to identify on the image specific features of interest on the cartridge case. This manual process is tedious and time consuming.

I have created an algorithm to automatically mask cartridge case images using Detectron2 on my own custom dataset. I have annotated the dataset manually via https://www.makesense.ai/ and exported the annotations as COCO JSON format. The cartridge case dataset can be accessed from https://www.kaggle.com/datasets/dnnpy1/tracks-on-bullet-cartridges.

Order of masking:
1.	The breech-face impression (red)
2.	The aperture shear (green)
3.	The firing pin impression (purple)
4.	The firing pin drag (light blue) 
5.	The direction of the firing pin drag (blue arrow)

![image](https://github.com/mldriven/Masking-Cartridge-Case-Images-with-Custom-Annotations/assets/64216950/1b8f6ba0-7dd7-4cde-bd00-e3ebb5b3448c)

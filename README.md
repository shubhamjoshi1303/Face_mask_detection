# Face_mask_detection
face mask detection using yolov5x model to train custom dataset and obtain weights to detect and deduce whether people are wearing a face mask or not , also gives estimated accuracy of the assumption . Weights obtained can then be used for real time face mask detection


Create three folders (train,val,test)
• Add images to these three folders (train – 100images, val – 50 images)(images to include both with
mask and without mask people)(leave test folder blank)
• (YOU CAN INCREASE THE NUMBER OF IMAGES IN BOTH FOLDERS TO GET BETTER ACCURACY)
• From this google drive link https://drive.google.com/drive/folders/1hGk-Eo-ZMQmwt_C4mJ3-
grqXkN5vIT0D?usp=sharing, there is one one folder called as download these images, download the
images from this folder (photos of people wearing mask and not wearing mask)(rename all images in
numerical order to avoid confusion [1.jpg to 200.jpg])
• Label these images(or annotate these images) using an online annotation tool/website called as
“makesense.ai”
• Create two labels mask and no_mask
• Label all the images
• Then click on actions , click on export annotations, select zip package containing yolo format and
then export
• We get a .zip file
• Extract it to a new folder (we get all the annotations as .txt files)
• In yolo v5 folder, in data folder we can find “coco128.yaml”, download it, rename it to custom.yaml
and then make changes to it (changes are mentioned in next step)
• Remove those 80 classes and give two classes (mask and no_mask)
• Add folders train and val in your drive
• Change the train and val folders path inside it (search for these two folders path and then put it in
the custom.yaml file)
• Upload the “custom.yaml” file back to the data folder in yolov5

## Project Title : Advanced AI-driven Defect Detection Solutions for Manufacturing Excellence
### Team Name : MechDefect Solutions              

### Project Objectives : 
(1) Develop AI-powered defect detection and classification solutions for industries that cater to the initial stages of manufacturing. <br>

(2) Leverage transfer learning by training our models on different processes (like casting, mining etc) gaining knowledge from one and applying it to other processes. <br>
***
###  Object Detection Model


This model detects and segments relevant components (by creating bounding boxes) from an image. For this, we have fine-tuned the **RetinaNet** with **ResNet50** backbone architecture on our custom dataset. For the sake of this project, we focused on (1) image inputs and (2) single class (pump impeller) detection with the assumption that every image can atmost have one pump impeller.

<img width="463" alt="Screenshot 2023-11-06 at 10 09 29 AM" src="https://github.com/codeWITHswap/ME781_SML/assets/81500272/4a2c5f93-4482-4007-bf63-517bb84a42d5">


***
### Defect Detection Model

This model leverages the VGG16 architecture for the transfer learning process and categorizes the pump impeller as either being "Defective" or "OK".

<img width="702" alt="Screenshot 2023-11-06 at 10 14 57 AM" src="https://github.com/codeWITHswap/ME781_SML/assets/81500272/7ca64655-904c-41e8-a4af-493fb699acf0">


***
### Defect Classification Model

This model leverages the VGG16 architecture for the transfer learning process and for the sake of our project, we have considered 6 different types of defects : Crazing, Inclusions, Patches, Scratches, Pitted and Rolled.

<img width="702" alt="Screenshot 2023-11-06 at 10 15 30 AM" src="https://github.com/codeWITHswap/ME781_SML/assets/81500272/4f8edddf-3da3-4b96-bef8-e0d056439857">


***

All of these models have been made available for inference on the following space using Gradio : https://huggingface.co/spaces/codeWITHswap/gradio-ME781-project 





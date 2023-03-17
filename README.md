# Deep Learning Use Case in Healthcare
This project is part of a `Hackathon` from **Deep Learning for Computer Vision(DLCV)** at IISc.

`Match patients from before and after eye-operation images.`

Runners Up -  DLCV Hackathon 2021

# Introduction
To support underprivileged individuals, an NGO finances cataract surgeries at eye hospitals and releases funds based on the number of free surgeries performed. To ensure that only valid surgeries are funded, the NGO currently requests eye hospitals to submit pre-operation (pre-op) and post-operation (post-op) photographs of each patient's face as proof that the surgery has been performed. The NGO also needs to verify that the same patient's photographs are not being submitted repeatedly for fraudulent fund claims. Therefore, they require a system that can compare these images and identify cases with a high likelihood of fraud, which can then be manually investigated further.
# Problem statement

The NGO requires a reliable system for comparing pre and post-operative photographs (as shown in the figure below) and accurately identifying the same patient. However, the post-operative images contain a patch covering a portion of the patient's face, which poses a challenge for existing facial recognition algorithms that require a full view of the face. Therefore, a solution must be found to detect and match patients from pre and post-operative images, even when a section of the face is obscured by a patch.

Sample Image:
<img width="600" alt="Capture" src="https://user-images.githubusercontent.com/81372735/225899617-c5dcbccf-d8b3-4e48-a8ba-a08e869980df.PNG">


# Brief Approach
- Created two classes {1: True pair , 0: Fake Pair}
- Used a Siamese Network where image-pairs were fed.
- Weights of the model were frozen during training. Only the last Feed Forward layer was finetuned.
- Different ratios of True and Fake Pair were passed to make the model robust.

`Kindly refer to the attached report(pdf) for more details`









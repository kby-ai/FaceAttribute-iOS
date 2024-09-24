<p align="center">
  <a href="https://play.google.com/store/apps/dev?id=7086930298279250852" target="_blank">
    <img alt="" src="https://github-production-user-asset-6210df.s3.amazonaws.com/125717930/246971879-8ce757c3-90dc-438d-807f-3f3d29ddc064.png" width=500/>
  </a>  
</p>

#### 📚 Product & Resources - [Here](https://github.com/kby-ai/Product)
#### 🛟 Help Center - [Here](https://docs.kby-ai.com)
#### 💼 KYC Verification Demo - [Here](https://github.com/kby-ai/KYC-Verification-Demo-Android)
#### 🙋‍♀️ Docker Hub - [Here](https://hub.docker.com/u/kbyai)

# FaceAttribute-iOS

## Overview

This repository integrates several facial recognition technologies, including 3D passive face liveness detection, face recognition, automatic face capture, and analysis of various face attributes such as age, gender, face quality, facial occlusion, eye closure, and mouth opening.

The system utilizes Face Liveness Detection technology to generate a real-time liveness score based on a single image captured by the camera. 

Additionally, this demo offers Face Recognition capabilities, enabling enrollment from a gallery and real-time identification of faces captured by the camera.

This repository features an automatic Face Capture function that verifies various facial attributes, such as face quality, facial orientation (yaw, roll, pitch), facial occlusion (e.g., mask, sunglass, hand over face), eye closure, mouth opening, and the position of the face within the region of interest (ROI).

Moreover, the repository can compute scores for different face attributes from a gallery image, including liveness, face orientation (yaw, roll, pitch), face quality, luminance of the face, facial occlusion, eye closure, mouth opening, age, and gender.

> In this repository, we integrated KBY-AI's Premium Face Mobile SDK into iOS platform.</br>
### ◾FaceSDK(Mobile) Details

  | Basic      | Standard | 🔽 Premium |
  |------------------|------------------|------------------|
  | Face Detection        | Face Detection    | <b>Face Detection</b> |
  | Face Liveness Detection        | Face Liveness Detection    | <b>Face Liveness Detection</b> |
  | Pose Estimation        | Pose Estimation    | <b>Pose Estimation</b> |
  |         | Face Recognition    | <b>Face Recognition</b> |
  |         |         | <b>68 points Face Landmark Detection</b> |
  |         |         | <b>Face Quality Calculation</b> |
  |         |         | <b>Face Occlusion Detection</b> |
  |         |         | <b>Eye Closure Detection</b> |
  |         |         | <b>Age, Gender Estimation</b> |

### ◾FaceSDK(Mobile) Product List
  | No.      | Repository | SDK Details |
  |------------------|------------------|------------------|
  | 1        | [Face Liveness Detection - Android](https://github.com/kby-ai/FaceLivenessDetection-Android)    | Basic SDK |
  | 2        | [Face Liveness Detection - iOS](https://github.com/kby-ai/FaceLivenessDetection-iOS)    | Basic SDK |
  | 3        | [Face Recognition - Android](https://github.com/kby-ai/FaceRecognition-Android)    | Standard SDK |
  | 4        | [Face Recognition - iOS](https://github.com/kby-ai/FaceRecognition-iOS)    | Standard SDK |
  | 5        | [Face Recognition - Flutter](https://github.com/kby-ai/FaceRecognition-Flutter)        | Standard SDK |
  | 6        | [Face Recognition - React-Native](https://github.com/kby-ai/FaceRecognition-React-Native)        | Standard SDK |
  | 7        | [Face Attribute - Android](https://github.com/kby-ai/FaceAttribute-Android)        | Premium SDK |
  | ➡️        | <b>[Face Attribute - iOS](https://github.com/kby-ai/FaceAttribute-iOS)</b>        | <b>Premium SDK</b> |
  | 9        | [Face Attribute - Flutter](https://github.com/kby-ai/FaceAttribute-Flutter)        | Premium SDK |

 > To get Face SDK(server), please visit products [here](https://github.com/kby-ai/Product).<br/>

## Download on the App Store

<a href="https://apps.apple.com/us/app/kby-ai-face-recognition/id6448648922" target="_blank">
  <img alt="" src="https://user-images.githubusercontent.com/125717930/235276083-d20fe057-214d-497c-a431-4569bbeed2fe.png" height=80/>
</a>

## Screenshots
<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/66a5037d-426c-4ea0-8e65-db0f456360d0" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/2214b69f-39e6-4f3f-9cd9-731fa869c57c" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/2d119006-1f2f-4852-aa99-7b3f81e6d73a" width=240/>
</p>

<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/e4f1dc19-a685-45ff-80a4-95a59e5f9f81" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/c545b864-3915-4099-8bf5-9868f979b3d7" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/932bd515-572b-4e0e-94bc-30a6f06511c7" width=240/>
</p>

<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/4a270e7c-8840-44ea-8e55-9625bd70f196" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/6383b0b8-7ada-4f50-ab77-bf60e8c09580" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/159cc87d-82cc-407d-9948-9b7825f5902e" width=240/>
</p>

## SDK License

The face attribute project relies on KBY-AI's SDK, which requires a license for each bundle ID.

- The code below shows how to use the license: https://github.com/kby-ai/FaceAttribute-iOS/blob/3e377692dcd101067ba57033db8a43a84ceced28/FaceAttribute/ViewController.swift#L42-L51

- To request a license, please contact us:</br>
🧙`Email:` contact@kby-ai.com</br>
🧙`Telegram:` [@kbyai](https://t.me/kbyai)</br>
🧙`WhatsApp:` [+19092802609](https://wa.me/+19092802609)</br>
🧙`Skype:` [live:.cid.66e2522354b1049b](https://join.skype.com/invite/OffY2r1NUFev)</br>
🧙`Facebook:` https://www.facebook.com/KBYAI</br>

## About SDK

### 1. Set up
- Copy the SDK (facesdk.framework folder) to the root folder of your project.

- Add SDK framework to the project in xcode

> Project Navigator -> General -> Frameworks, Libraries, and Embedded Content

![image](https://user-images.githubusercontent.com/125717930/231925359-ef30b3c0-d2d9-4b32-ae57-80b42b021b91.png)

- Add the bridging header to your project settings

> Project Navigator -> Build Settings -> Swift Compiler - General

![image](https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/5104749e-807b-47ce-b885-88fce65bfb77)

### 2. Initializing an SDK

- Step One

  To begin, you need to activate the SDK using the license that you have received.
  ```swift
  FaceSDK.setActivation("...") 
  ```
  If activation is successful, the return value will be SDK_SUCCESS. Otherwise, an error value will be returned.

- Step Two

  After activation, call the SDK's initialization function.
  ```swift
  FaceSDK.initSDK()
  ```
  If initialization is successful, the return value will be SDK_SUCCESS. Otherwise, an error value will be returned.

### 3. SDK Classes

  - FaceBox
  
    This class represents the output of the face detection function and can be utilized in template creation functions.

    | Feature| Type | Name |
    |------------------|------------------|------------------|
    | Face rectangle        | int    | x1, y1, x2, y2 |
    | Face angles (-45 ~ 45)        | float    | yaw, roll, pitch |
    | Liveness score (0 ~ 1)        | float    | liveness |
    | Face quality (0 ~ 1)        | float    | face_quality |
    | Face luminance (0 ~ 255)       | float    | face_luminance |
    | Face occlusion (0 ~ 1)       | float    | face_occlusion |
    | Eye closure (0 ~ 1)       | float    | left_eye, right_eye |
    | Mouth opening (0 ~ 1)       | float    | face_mouth_opened |
    | Age, gender        | int    | age, gender |
    | 68 points facial landmark        | Data    | landmark |
  
    > 68 points facial landmark
    
    <img src="https://user-images.githubusercontent.com/125717930/235560305-ee1b6a39-5dab-4832-a214-732c379cabfd.png" width=500/>

  - FaceDetectionParam
  
    This class serves as the input parameter for face detection, enabling various processing functionalities such as face liveness detection, eye closure checking, facial occlusion checking, mouth opening checking, and age and gender estimation.

    | Feature| Type | Name |
    |------------------|------------------|------------------|
    | Check liveness        | bool    | check_liveness |
    | Check eye closure        | bool    | check_eye_closeness |
    | Check face occlusion        | bool    | check_face_occlusion |
    | Check mouth opening        | bool    | check_mouth_opened |
    | Estimate age, gender        | bool    | estimate_age_gender |
    
### 4. SDK APIs
#### - Face Detection

  The Face SDK provides a unified function for detecting faces, enabling multiple functionalities such as liveness detection, face orientation (yaw, roll, pitch), face quality, facial occlusion, eye closure, mouth opening, age, gender, and facial landmarks.

  The function can be used as follows:

  ```swift
  let faceBoxes = FaceSDK.faceDetection(image, param: param)
  ```

  This function requires two parameters: a UIImage object and a FaceDetectionParam object that enables various processing functionalities.

  The function returns a list of FaceBox objects.

#### - Create Templates

  The FaceSDK provides a function that can generate a template from a UIImage image. This template can then be used to verify the identity of the individual captured in the image.

  ```swift
  let templates = FaceSDK.templateExtraction(image, faceBox: faceBox)
  ```

  The SDK's template extraction function takes two parameters: a UIImage object and an object of FaceBox. 

  The function returns a Data, which contains the template that can be used for person verification.

#### - Calculation similiarity

  The "similarityCalculation" function takes a byte array of two templates as a parameter. 

  ```swift
  let similarity = FaceSDK.similarityCalculation(templates, templates2: personTemplates)
  ```

  It returns the similarity value between the two templates, which can be used to determine the level of likeness between the two individuals.

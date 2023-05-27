<p align="left">
  <img src="https://user-images.githubusercontent.com/125717930/225975240-24b9a8ad-8cc6-4d5f-9a91-1435951b0bd7.png" width="120" alt="Nest Logo" />
</p>

👏  We have published the Face Livness Detection, Face Recognition SDK and ID Card Recognition SDK for the server.

  - [FaceLivenessDetection-Docker](https://github.com/kby-ai/FaceLivenessDetection-Docker)

  - [FaceRecognition-Docker](https://github.com/kby-ai/FaceRecognition-Docker)

  - [IDCardRecognition-Docker](https://github.com/kby-ai/IDCardRecognition-Docker)

# FaceAttribute-iOS

## Introduction

This demo project integrates several facial recognition technologies, including 3D passive face liveness detection, face recognition, automatic face capture, and analysis of various face attributes such as age, gender, face quality, facial occlusion, eye closure, and mouth opening.

The system utilizes Face Liveness Detection technology to generate a real-time liveness score based on a single image captured by the camera. 

Additionally, the demo offers Face Recognition capabilities, enabling enrollment from a gallery and real-time identification of faces captured by the camera.

The demo also features an automatic Face Capture function that verifies various facial attributes, such as face quality, facial orientation (yaw, roll, pitch), facial occlusion (e.g., mask, sunglass, hand over face), eye closure, mouth opening, and the position of the face within the region of interest (ROI).

Moreover, the demo can compute scores for different face attributes from a gallery image, including liveness, face orientation (yaw, roll, pitch), face quality, luminance of the face, facial occlusion, eye closure, mouth opening, age, and gender.

> The demo is integrated with KBY-AI's Premium Face Mobile SDK.

  | Basic      | Standard | Premium |
  |------------------|------------------|------------------|
  | Face Detection        | Face Detection    | Face Detection |
  | Face Liveness Detection        | Face Liveness Detection    | Face Liveness Detection |
  | Pose Estimation        | Pose Estimation    | Pose Estimation |
  |         | Face Recognition    | Face Recognition |
  |         |         | 68 points Face Landmark Detection |
  |         |         | Face Quality Calculation |
  |         |         | Face Occlusion Detection |
  |         |         | Eye Closure Detection |
  |         |         | Age, Gender Estimation |

> For other solutions, please explore the following:
> - [Face Liveness Detection - Android(Basic SDK)](https://github.com/kby-ai/FaceLivenessDetection-Android)
> - [Face Liveness Detection - iOS(Basic SDK)](https://github.com/kby-ai/FaceLivenessDetection-iOS)
> - [Face Recognition - Android(Standard SDK)](https://github.com/kby-ai/FaceRecognition-Android)
> - [Face Recognition - iOS(Standard SDK)](https://github.com/kby-ai/FaceRecognition-iOS)
> - [Face Attribute - Android(Premium SDK)](https://github.com/kby-ai/FaceAttribute-Android)
> - [Face Attribute - iOS(Premium SDK)](https://github.com/kby-ai/FaceAttribute-iOS)

## Download on the App Store

<a href="https://apps.apple.com/us/app/kby-ai-face-recognition/id6448648922" target="_blank">
  <img alt="" src="https://user-images.githubusercontent.com/125717930/235276083-d20fe057-214d-497c-a431-4569bbeed2fe.png" height=80/>
</a>

## Screenshots
<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/eaeb83b5-fb22-4c20-986c-bc8c8597d8a4" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/2214b69f-39e6-4f3f-9cd9-731fa869c57c" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/2d119006-1f2f-4852-aa99-7b3f81e6d73a" width=240/>
</p>

<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/02a619de-bfd8-47ab-abc5-2365e9c87993" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/8e1d34a5-8171-4334-9a44-e761460f63cd" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/1b04943f-c00a-4632-857a-8b53485c962e" width=240/>
</p>

<p float="left">
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/4a270e7c-8840-44ea-8e55-9625bd70f196" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/63c283a2-d25d-46c9-82bb-2b9c7abd5b2c" width=240/>
  <img src="https://github.com/kby-ai/FaceAttribute-iOS/assets/125717930/ff9758fd-51ed-4c78-a1fd-074fed5a33e4" width=240/>
</p>

## SDK License

The face attribute project relies on kby-ai's SDK, which requires a license for each bundle ID.

- The code below shows how to use the license: https://github.com/kby-ai/FaceAttribute-iOS/blob/3e377692dcd101067ba57033db8a43a84ceced28/FaceAttribute/ViewController.swift#L42-L51

- To request a license, please contact us:
  ```
  Email: contact@kby-ai.com

  Telegram: @kbyai

  WhatsApp: +19092802609

  Skype: live:.cid.66e2522354b1049b
  ```

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
  ```
  FaceSDK.setActivation("...") 
  ```
  If activation is successful, the return value will be SDK_SUCCESS. Otherwise, an error value will be returned.

- Step Two

  After activation, call the SDK's initialization function.
  ```
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

  ```
  let faceBoxes = FaceSDK.faceDetection(image, param: param)
  ```

  This function requires two parameters: a UIImage object and a FaceDetectionParam object that enables various processing functionalities.

  The function returns a list of FaceBox objects.

#### - Create Templates

  The FaceSDK provides a function that can generate a template from a UIImage image. This template can then be used to verify the identity of the individual captured in the image.

  ```
  let templates = FaceSDK.templateExtraction(image, faceBox: faceBox)
  ```

  The SDK's template extraction function takes two parameters: a UIImage object and an object of FaceBox. 

  The function returns a Data, which contains the template that can be used for person verification.

#### - Calculation similiarity

  The "similarityCalculation" function takes a byte array of two templates as a parameter. 

  ```
  let similarity = FaceSDK.similarityCalculation(templates, templates2: personTemplates)
  ```

  It returns the similarity value between the two templates, which can be used to determine the level of likeness between the two individuals.

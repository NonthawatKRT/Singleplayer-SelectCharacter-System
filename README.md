# Singleplayer-SelectCharacter-System
This is StarterKit for making SinglePlayer Character Selection

**This Project Using**
- UnityEditor 2022.3.62f1
- TextMesh Pro
- Starter Assets - ThirdPerson 1.1.6 (released on Sep 11, 2024)
- glTFast 6.13.0 https://github.com/atteneder/glTFast
- UniVRM 0.129.3 https://github.com/vrm-c/UniVRM
- Unity-UI-Rounded-Corners v3.0.2 candidate https://github.com/ReForge-Mode/Unity_UI_Rounded_Corners

**Adding More Character**

- To Add more Character Avatar first you need to create you import you new character

  <img width="1638" height="192" alt="image" src="https://github.com/user-attachments/assets/0af900dc-e7f5-44d4-8100-0d630764e6bb" />


- if yours character dont have texture and materails you need to create folder to extract the materails and textures

  <img width="1638" height="208" alt="image" src="https://github.com/user-attachments/assets/20cc3e8f-d946-4c78-a9f4-faba496365b4" />

- Extract materails and texture to folder

  <img width="400" height="250" alt="image" src="https://github.com/user-attachments/assets/1a334a5e-1087-4b01-b509-c12ff0283ba9" />

- Change Rig Animation Type to Humanoid

  <img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/08100210-f5a1-4451-a970-55d7f9693d37" />

- Duplicate character form character list and replace old character modle with new one

  - **Old version**
    
    <img width="300" height="450" alt="image" src="https://github.com/user-attachments/assets/f133ff31-b948-4ffc-9833-4e1b45c904cc" />

  - **New version**
    
    <img width="300" height="450" alt="image" src="https://github.com/user-attachments/assets/3cc8c161-84c1-4593-9ebe-f4bdd2332cab" />

- Apply Avata to NewCharacter Animators
  - Put the Avatar form you newcharacter model in to the avatar field in animator component in playerAmature
 
    <img width="2559" height="1235" alt="image" src="https://github.com/user-attachments/assets/e40c7cf5-d2f8-47e9-8ad5-d8de298cce30" />

    *If you can't find the avatar component form your newcharacter model plese check you have change the animation type to Humanoid and Change Avatar Definition field to Create Form This Avatar and hit Apply

  - Assign your newcharacter to the Characters list in MainmenuController
    <img width="2559" height="716" alt="image" src="https://github.com/user-attachments/assets/ca7fa37f-d5d9-4fbc-9276-cd5ddf98fbd1" />

- Modify Character Slot Canvas Add you new Character card

  <img width="1956" height="644" alt="image" src="https://github.com/user-attachments/assets/77366f8a-c860-4983-b950-92b6fceb3368" />

- Increase The Character Index in the Card Button
  *For me now this is the 4 index
  
  <img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/43242bcb-8053-482e-b004-a360ed790b4d" />

- Go to mainmap scene and do the same thing to the characterList

  - replace old character model with yours
  
    <img width="1953" height="1226" alt="image" src="https://github.com/user-attachments/assets/82cde35c-fa84-44a5-be13-06a2b2495746" />

  - Change Avatar in animator component of PlayerAmature
 
    <img width="2559" height="1258" alt="image" src="https://github.com/user-attachments/assets/e234e645-a41d-41de-9678-91cd041b7a7e" />

  - Add your newcharacter to character list in GameManager
 
    <img width="2559" height="657" alt="image" src="https://github.com/user-attachments/assets/020212bf-cfa6-4a84-a74a-39b2d3cb807d" />




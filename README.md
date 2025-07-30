# Singleplayer Select Character System

A **Starter Kit** for implementing a character selection system in single-player Unity projects.

---

## 📦 Project Details

This project is built using:

- **Unity Editor**: 2022.3.62f1  
- **TextMesh Pro**
- **Starter Assets – Third Person**: v1.1.6 (Released Sep 11, 2024)  
- **glTFast**: [v6.13.0](https://github.com/atteneder/glTFast)  
- **UniVRM**: [v0.129.3](https://github.com/vrm-c/UniVRM)  
- **Unity UI Rounded Corners**: [v3.0.2 (candidate)](https://github.com/ReForge-Mode/Unity_UI_Rounded_Corners)

---

## ➕ Adding a New Character

Follow the steps below to add a new character avatar into the system.

### 1. Import Your Character

Import your character model into the Unity project.

![Import Character](https://github.com/user-attachments/assets/0af900dc-e7f5-44d4-8100-0d630764e6bb)

### 2. Extract Materials and Textures

If your model doesn’t include textures or materials:
- click the model in the inspector you will see → **Materials...**
- Choose or create a folder for extract Materails and Textures.

![Extract Materials Option](https://github.com/user-attachments/assets/20cc3e8f-d946-4c78-a9f4-faba496365b4)  
![Extract Materials](https://github.com/user-attachments/assets/1a334a5e-1087-4b01-b509-c12ff0283ba9)

### 3. Set Rig Type to Humanoid

Go to the **Rig** tab in the model’s Inspector, and:

- Set **Animation Type** to **Humanoid**
- Click **Apply**

![Set to Humanoid](https://github.com/user-attachments/assets/08100210-f5a1-4451-a970-55d7f9693d37)

### 4. Replace Character in Character List

Duplicate one of the existing character prefabs and replace the model with your new one.

**Old Character:**  
<img width="300" height="450" src="https://github.com/user-attachments/assets/f133ff31-b948-4ffc-9833-4e1b45c904cc" />

**New Character:**  
<img width="300" height="450" src="https://github.com/user-attachments/assets/3cc8c161-84c1-4593-9ebe-f4bdd2332cab" />

### 5. Assign Avatar to Animator

Assign the avatar from your model to the **Animator** component of the `PlayerArmature`.

![Assign Avatar](https://github.com/user-attachments/assets/e40c7cf5-d2f8-47e9-8ad5-d8de298cce30)

> 🛠 **Tip:** If the Avatar field doesn’t appear, ensure:
> - The model’s **Animation Type** is set to **Humanoid**
> - The **Avatar Definition** is set to **Create From This Model**
> - Click **Apply** again.

### 6. Add Character to Main Menu

- Go to the `MainMenuController` object
- Add your new character to the **Characters** list

![Add to MainMenuController](https://github.com/user-attachments/assets/ca7fa37f-d5d9-4fbc-9276-cd5ddf98fbd1)

### 7. Update Character Slot UI

In the character selection canvas:

- Duplicate an existing character card
- Update it to reference your new character
- Adjust the **Character Index** in the card’s button (e.g., index 4)

![Character Card](https://github.com/user-attachments/assets/77366f8a-c860-4983-b950-92b6fceb3368)  
![Character Index](https://github.com/user-attachments/assets/43242bcb-8053-482e-b004-a360ed790b4d)

### 8. Update Main Map Scene

Repeat similar steps in the `MainMap` scene:

- Replace the old character model with your new one in the scene

![Replace Model](https://github.com/user-attachments/assets/82cde35c-fa84-44a5-be13-06a2b2495746)

- Update the Animator’s **Avatar** in the `PlayerArmature`

![MainMap Avatar](https://github.com/user-attachments/assets/e234e645-a41d-41de-9678-91cd041b7a7e)

- Add your character to the **Character List** in the `GameManager`

![GameManager Character List](https://github.com/user-attachments/assets/020212bf-cfa6-4a84-a74a-39b2d3cb807d)

---

## ✅ You're Done!

Your new character should now be selectable in the main menu and appear correctly in the game.

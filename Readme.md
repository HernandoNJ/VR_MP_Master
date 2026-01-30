# 🎮 Unity VR MP Project Setup

## Description

Project integrating 3 Unity templates:

- **Multiplayer Third Person Gameplay Template**
- **VR Multiplayer Template**
- **VR Template**

## Contact

[Discord](https://discord.gg/Jr4vmVKs)    [LinkedIn](https://www.linkedin.com/in/hernandonj/)    [Medium](https://medium.com/@hernandonj)

---

## Index

[**Requirements**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-requirements)

[**Installation**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-installation)

1. [Clone the repository and install git lfs](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#1-clone-the-repository-and-install-git-lfs)
2. [Templates and Samples folders](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#2-templates-and-samples-folders)
3. [Open in Unity](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#3-open-in-unity)
4. [Verify Installation](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#4-verify-installation)

[**Project structure**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-project-structure)

[**Development Workflow**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-development-workflow)

[**Documentation**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#documentation)

[**Known issues**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#known-issues)

---

## 📋 Requirements

- Unity 6000.3.5f2 LTS
- Git
- 2 GB free disk space (~1 GB for templates)

## 🚀 Installation

### 1. Clone the repository and install git lfs

- Clone project using git or GitHub
    
    `git clone https://github.com/HernandoNJ/VR_MP_Master.git`
    
- In the local repository folder, using git or GitHub, initialize gif lfs
    
    `git lfs install`
    

---

### 2. Templates and Samples folders

- Download the Templates: [download link](https://drive.google.com/file/d/1HGPdIHZtcX4ISzSaFVj3xhETKf401M2s/view?usp=sharing)
- Unzip
- Copy the content from the **MPTPVR templates** folder in the project’s root **Assets folder** (Templates, Samples and their .meta files).
    
    *If a warning about replacing files and/or folders is displayed, replace the folder.*
    
    **Don’t modify any assets from Templates folder. If required any assets from there, copy, paste and rename them in another location of the project.**
    

---

### 3. Open in Unity

1. Open **Unity Hub**
2. **Add** → Add Project from disk
    1. Select project folder
3. **Open**
4. Wait for initial loading
    
    *If a warning saying “Enter Safe Mode” is displayed, check for this in [known issues](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#known-issues)*
    
5. When the project is open
    
    *If a warning: `GameplayKitInputSystem_Actions.cs(1210,21): is in conflict with …` is displayed, check for this in [known issues](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#known-issues)*
    

---

### 4. Verify Installation

- Verify if `Assets/Templates/` and `Assets/Templates/` have their own content
- No errors in Unity console
- Project scenes working properly

---

## 📁 Project Structure

```
Assets/
├── Templates/          # ⚠️ DO NOT MODIFY - Reference only
│   ├── Characters/     #    Copy from here to Development/
│   ├── Environment/
│   └── UI/
├── Development/        # ✅ Your work goes here
│   ├── Characters/     #    Modified/customized assets
│   ├── Levels/
│   └── Prefabs/
├── Scripts/
└── Scenes/
```

---

## 🔧 Development Workflow

### Avoid this:

`Modify Assets/Templates/Character.prefab`

### ✅ DO this instead:

```markdown
1. Copy `Assets/Templates/Character.prefab`  
2. Paste into `Assets/Development/Characters/`  
3. Rename to `MyCharacter.prefab`  
4. Modify freely  
```

---

## Documentation

[**Multiplayer Third Person Gameplay Template**](https://docs.unity3d.com/Packages/com.unity.template.multiplayer-third-person-gameplay@1.0/manual/index.html)

[**VR Multiplayer Template**](https://docs.unity3d.com/Packages/com.unity.template.vr-multiplayer@2.0/manual/index.html)

[**VR Template**](https://docs.unity3d.com/Packages/com.unity.template.vr@9.2/manual/index.html)

---

### Known issues

**Warning: GameplayInputSystem_Actions**

`Assets\Core\Scripts\Runtime\Framework\GameplayKitInputSystem_Actions.cs(1210,21): warning CS0436: The type 'GameplayInputSystem_Actions' in …. conflicts with …`

- Remove the `Assets/Core` folder in the Unity editor

---

**Project Loading**

**Warning: Enter safe mode warning**

- Click on Continue

---

**Warning: Multiplayer Services**

Message informing about incompatibility of Multiplayer Services, Lobby and Realy with Unity Multiplayer Services SDK

- Click on close

---

**Error: Samples namespace**

Missing assembly reference in `Assets\Templates\VRMP\VRMPAssets\Scripts\Gameplay\MessageBoard\NetworkMessageBoard.cs(5,42):`

Go to the Package Manager and import the following samples from these packages :

 **XRIT 3.3.1**

- Starter assets
- Hands interaction demo
- Spatial Keyboard
- World space UI

**XR Hands**

- Hands visualizer

---

**Issues in XR Plugin Management - Project validation - Android Tab**

**Warning: [OpenXR] At least one interaction profile must be added.**

- Click on Edit
- In the Enabled interaction profiles section:
    - Click on +
    - Select the Oculus Touch Controller Profile

---

**Warning: [XR] [Spatial Keyboard] TextMesh Pro - TMP Essentials must be installed for this sample**

**Option 1**

- Click on Edit
- Click on Import TMP Essentials

**Option 2**

- Go to Window/TextMeshPro/Import TMP Essentials Resources
- Click on Import

---

[Back to top](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-unity-vr-mp-project-setup)
# 🎮 Unity VR MP Project Setup

### Description

Project integrating 3 Unity templates:

- **Multiplayer Third Person Gameplay Template**
- **VR Multiplayer Template**
- **VR Template**

## Index

[**Requirements**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-requirements)

[**Installation**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-installation)

[Clone the repository and install git lfs](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#1-clone-the-repository-and-install-git-lfs)

[Templates](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#2-templates)

[Open in Unity](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#3-open-in-unity)

[Verify Installation](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#4-verify-installation)

[**Project structure**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-project-structure)

[**Development Workflow**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#-development-workflow)

[**Known issues**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#known-issues)

[**Documentation**](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#documentation)

[Discord](https://github.com/HernandoNJ/VR_MP_Master?tab=readme-ov-file#discord)

## 📋 Requirements

- Unity 6000.3.5f2 LTS
- Git
- 2 GB free disk space (~1 GB for templates)

## 🚀 Installation

### 1. Clone the repository and install git lfs

`git clone https://github.com/HernandoNJ/VR_MP_Master.git`

`cd VR_MP_Master`

`git lfs install`

### 2. Templates

**REQUIRED**

- Download the Templates: [download link](https://drive.google.com/file/d/1t8dojugnnsZZUnzntCI1gT9GDuAbJVmw/view?usp=sharing)
- Unzip
- Add the Templates folder and its .meta file into the root Assets folder

**Don’t modify any assets from Templates folder. Copy, paste and rename the assets in another location of the project.**

### 3. Open in Unity

1. Open **Unity Hub**
2. **Add** → Add Project from disk
    1. Select project folder
3. **Open**
4. Wait for initial import

### 4. Verify Installation

✅ You should see:

- `Assets/Templates/` with content
- No errors in Unity console
- Project scenes working properly

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

## 🔧 Development Workflow

### ❌ DON'T do this:

`Modify Assets/Templates/Character.prefab`

### ✅ DO this instead:

```markdown
1. Copy `Assets/Templates/Character.prefab`  
2. Paste into `Assets/Development/Characters/`  
3. Rename to `MyCharacter.prefab`  
4. Modify freely  
```

## Known issues

### **Enter safe mode warning - project initialization**

- Click on Continue

### **Warning: Multiplayer Services**

Message informing about incompatibility of Multiplayer Services, Lobby and Realy with Unity Multiplayer Services SDK

- Click on close

### **Error: Samples namespace**

`Assets\Templates\VRMP\VRMPAssets\Scripts\Gameplay\MessageBoard\NetworkMessageBoard.cs(5,42): error CS0234: The type or namespace name 'Samples' does not exist in the namespace 'UnityEngine.XR.Interaction.Toolkit' (are you missing an assembly reference?)`

Go to the Package Manager

Import the following samples from the packages mentioned:

 **XRIT 3.3.1**

- Starter assets
- Hands interaction demo
- Spatial Keyboard
- World space UI

**XR Hands**

- Hands visualizer

### **Warning: GameplayInputSystem_Actions**

`Assets\Core\Scripts\Runtime\Framework\GameplayKitInputSystem_Actions.cs(1210,21): warning CS0436: The type 'GameplayInputSystem_Actions' in …. conflicts with the imported type 'GameplayInputSystem_Actions' in 'Blocks.Gameplay.Core, Version=0.0.0.0, …`

- Remove the `Assets/Core` folder in the Unity editor

### Issues in XR Plugin Management - Project validation - Android Tab

### **Warning: [OpenXR] At least one interaction profile must be added.**

- Click on Edit
- In the Enabled interaction profiles section:
    - Click on +
    - Select the Oculus Touch Controller Profile

### Warning: [XR] [Spatial Keyboard] TextMesh Pro - TMP Essentials must be installed for this sample

**Option 1**

- Click on Edit
- Click on Import TMP Essentials

**Option 2**

- Go to Window/TextMeshPro/Import TMP Essentials Resources
- Click on Import

## Documentation

- [**Multiplayer Third Person Gameplay Template**](https://docs.unity3d.com/Packages/com.unity.template.multiplayer-third-person-gameplay@1.0/manual/index.html)
- [**VR Multiplayer Template**](https://docs.unity3d.com/Packages/com.unity.template.vr-multiplayer@2.0/manual/index.html)
- [**VR Template**](https://docs.unity3d.com/Packages/com.unity.template.vr@9.2/manual/index.html)

### Discord

[Discord Link](https://discord.gg/Jr4vmVKs)
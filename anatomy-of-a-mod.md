# Anatomy of the Elemental Warfighter mod for Elden Ring

- What this mod does
See [Elemental Tank](https://www.nexusmods.com/eldenring/mods/4920)

- What will we be dissecting?

We will do a breadth-first tour of the entire tour. This will cover many aspects of mod-making at various levels of complexity, but obviously not all. There are also a whole host of tutorials available on the [Souls Modding Wiki](http://soulsmodding.wikidot.com/).

# A Note about Version Control

# A Note about the Environment

# Levels of Difficulty

- Replacing / Overriding Existing Animations
  - Mod Example: Idle / Walk / Run animations
- Editing Existing Animations
  - Modifying Animations with Blender
    - Exporting to Blender
    - High-level Blender workflow
    - Importing back into the game
  - Mod Example: Ghostflame Dodge
- Creating new Animation entries
  - Creating new TAEs
  - Editing TAEs
    - Interesting TAE Entries
      - Attacks (InvokeBulletBehavior / InvokeAttackBehavior)
      - Visual FX (SpawnOneShotFFX / SpawnFFX_Blade)
      - Animation Properties (AnimSpeedGradient / RootMotionReduction / RootMotionMultiplierEX)
      - IFrames and Cancellations (Jumptable Flag as Dodging, Cancel TAE's, InvokeDS3Poise)
      - Special Effects (AddSpEffect)
  - Modifying your BEHBND
    - Doing it manually
    - Doing it through ERClipGenerator
    - What does the Game Loop look like, roughly?
  - Exploring the state machines
  - Mod Example: Custom 1H Flame Art Zweihander moveset
- Creating Bullets, Attacks, Special Effects, and Behaviours
  - Reusing Player Character Behaviours
    - Bullets and InvokeBulletBehavior
    - Attacks and InvokeAttackBehavior
    - Mod Example: Dodge Stomp
    - Mod Example: Glintstone Pull
  - Using NPC Behaviours
    - Example: Draconic Tree Sentinel's AoE Lightning Strike
  - Behaviours without Coding: HKS Events
- HKS Editing
  - Instrumenting your Lua code: Discovering what gets triggered when
  - Debugging problematic code
  - Good code practices
  - Mod Example: Beast Claw on Land
  - Debugging HKS
    - Using common_define.hks and DSLuaDecompiler
    - Mod Example: Whirlwind on Sprint
- Modifying the game from the inside (C++ / Assembly)
  - Exploration with Cheat Engine
  - Writing decorators (MASM)
  - Notes about addresses
  - Notes on calling assembly from C++
  - Notes on calling C++ from assembly
  - General debugging and logging practices
  - Revisiting HKS: Triggering act() only Once in a SpEffect
  - Example: Blink Strike
- Editing Armor Models
  - Possible Issues
    - Global Rotation
    - No Weight Paint
    - Rubber-banding armor in-game: Vertex Groups which do not have a corresponding bone
    - Mod Example: Crucible Tree Knight armor with Crucible Axe Knight pauldrons
- Resources and Links
  - Yabber / WitchyBND
  - UXM Selective Unpacker
  - SkyrimFbxImporter
  - ModEngine 2
  - HkLibCLI
  - Havok Toolset (Fbx2Gltf)
  - Havok Content Tools
  - ERClipGenerator
  - DS Map Studio
  - DS Animation Studio
  - Elden Ring Debug Tool
  - Cheat Engine (Hexinton and TGA tables)
  - FLVER Editor
  - DSLuaDecompiler
  - Visual Studio
  - ElaDiDu's Script Data Exposer

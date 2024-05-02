# Anatomy of the Elemental Warfighter mod for Elden Ring

- What this mod does
See [Elemental Tank](https://www.nexusmods.com/eldenring/mods/4920)

- What will we be dissecting?

We will do a breadth-first tour of the entire tour. This will cover many aspects of mod-making at various levels of complexity, but obviously not all.

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
  - Exploring the state machines
  - Mod Example: Custom 1H Flame Art Zweihander moveset
- Creating Bullets, Attacks, Special Effects, and Behaviours
  - Reusing Player Character Behaviours
    - Bullets and InvokeBulletBehavior
    - Attacks and InvokeAttackBehavior
    - Example: Dodge Stomp
  - Using NPC Behaviours
    = Example: Draconic Tree Sentinel's AoE Lightning Strike
  - Behaviours without Coding: HKS Events
- HKS Editing
  - Instrumenting your code
  - Debugging and Tracing
  - Good practices when editing code
  - Example: Beast Claw on Land
- Modifying the game from the inside (C++ / Assembly)
  - Exploration with Cheat Engine
  - Writing decorators
  - Revisiting HKS: Triggering act() only Once in a SpEffect
  - Example: Blink Strike

- Tools
- Version Control
- Resources and Links
  - Yabber / WithcyBND
  - UXM Selective Unpacker
  - SkyrimFbxImporter
  - ModEngine 2
  - HkLibCLI
  - Havok Toolset
  - Havok Content Tools
  - ERClipGenerator
  - DS Map Studio
  - DS Animation Studio
  - Elden Ring Debug Tool
  - Cheat Engine (Hexinton and TGA tables)
  - MinHksLib
  - FLVER Editor
  - DSLuaDecompiler
  - etc.

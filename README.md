![My image](https://images.squarespace-cdn.com/content/v1/5808f139b8a79b2b73259cd1/1607704111422-6KOQLH1RIU83QTDH7N0A/P1000365%281%29.jpg?format=1000w)

# Cirklon Instrument Definitions
Instrument definitions for sequentix cirklon located in the `instruments` folder.
- **Roland JV-1080**
- **Korg Monologue** ([copied](http://forum.sequentix.com/viewtopic.php?p=18417&hilit=monologue#p18417) from sequentix forum user Ripperton)

---

# Additional Instructions

<details>
  <summary>JV-1080 Instrument Instructions</summary>

### Exposed Parameters
1. Mod Wheel (CC #1) 
2. Control 1 (CC #74 - assigned in JV-1080 system settings)
3. Control 2 (CC #71 - assigned in JV-1080 system settings)
4. Reverb EFX Level (CC #91)
5. Chorus EFX Level (CC #93)

### Notes
- The JV-1080 doesn’t expose very many parameters via MIDI CC. No filter cutoff, resonance, amp envelope where you might expect to find them. Instead, there are 3 assignable (including the mod wheel) parameters. 
- The 3 assignable parameters are patch-specific and configured in the JV-1080. 
- The instructions below are required to ensure the CONTROL 1 and CONTROL 2 parameters work correctly.
- The control values are set to CC#74, and CC#71 respectively. This is arbitrary and can be set to your preference––make sure to match the values in the cirklon match those set in JV-1080 the instructions below.

### JV-1080 Instructions (for performance mode)
1. Press **PERFORMANCE** button.
2. Press **SYSTEM** button.
3. Press **TONE SWITCH #3 (MIDI)** button. 
4. Use **Up/Down** arrow buttons to navigate page to “CONTROL ASSIGN”.
5. Use **Left/Right** arrow buttons to edit “Control 1” or “Control 2”.
6. Use **Jog Wheel** to set CC value for numbered control. 
    - For CONTROL 1: CC74 (usually used for filter cutoff)
    - For CONTROL 2: CC71 (usually used for filter resonance)
    - _NOTE: These values are arbitrary but match the included instrument definition. Must match cirklon track value CC#’s._
7. (Optional?) Press **UTILITY** -> **WRITE** -> **ENTER**.
</details>

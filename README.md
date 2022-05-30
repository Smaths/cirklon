# Cirklon Instrument Definitions
Instrument definitions for sequentix cirklon located in the `instruments` folder.

- **Elektron Machinedrum**
- **Korg Monologue** ([Copied](http://forum.sequentix.com/viewtopic.php?p=18417&hilit=monologue#p18417) from sequentix forum user Ripperton.)
- **Roland JV-1080**

![My image](https://images.squarespace-cdn.com/content/v1/5808f139b8a79b2b73259cd1/1607704111422-6KOQLH1RIU83QTDH7N0A/P1000365%281%29.jpg?format=1000w)

## Additional Info 

<details>
  <summary>Machinedrum Notes & Instructions (click to expand)</summary>
  
  ### MIDI Settings
  - The default MIDI settings are required for this instrument definition to work. Specifically the setting the `Base MIDI Channels` to 1-4.
  - Each sound machine (1-16) has a dedicated instrument in order to provide access to all the parameters. 
  - _Suggestion: On the cirklon, I have tracks 16-32 configured to match the machinedrums respective sound machines._
  
</details>

<details>
  <summary>Roland JV-1080 Notes & Instructions (click to expand)</summary>

  ### Exposed Parameters
  |Parameter|CC#|
  |--------|---|
  Mod Wheel | CC #1 
  Control 1 | CC #74 *
  Control 2 | CC #71 *
  Reverb EFX Level | CC #91
  Chorus EFX Level | CC #93
  
  \* _User-assigned in JV-1080 system settings. See instructions below._

  ### Notes
  - The JV-1080 doesn’t expose very many parameters via MIDI CC. No filter cutoff, resonance, amp envelope where you might expect to find them. Instead, there are 3 assignable (including the mod wheel) parameters. 
  - The 3 assignable parameters are patch-specific and configured in the JV-1080. 
  - The instructions below are required to ensure the CONTROL 1 and CONTROL 2 parameters work correctly.
  - The control values are set to CC#74, and CC#71. This is arbitrary and can be set to your preference––just make sure to match the values in the cirklon match those set in JV-1080 using the instructions below.

  ### JV-1080 Control CC# Assignment Instructions
  For performance mode, the mode I've been using on the JV-1080.
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
  
  ### Additional MIDI Properties
  These values should be set as followed on the in the System MIDI settings. 

  1. Press **PERFORMANCE** button.
  2. Press **SYSTEM** button.
  3. Press **TONE SWITCH #3 (MIDI)** button. 
  4. Use **Up/Down** arrow buttons to navigate pages.
  
  #### Page: PERFORM MIDI
  Control Channel - 16
  Clock - MIDI
  Stack - _shouldn't matter_

  #### Page: RECEIVE MIDI
  |Property|Value|
  |--------|-----|
  P.C | ON
  BnK | ON
  C.C | ON
  Vol | ON
  Hld | ON
  Bnd | ON
  Mod | ON
  Aft | ON
</details>

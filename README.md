# Expanded Mod Family GUI
The files required for the GUI in the lobby that displays all Expanded Mods and which are active.

## How to use
**1.** Copy all folders in your mod, overwrite files if needed (if you have an older version already in your mod, otherwise merge conflicting files).

**2.** Rename the **zzz_expanded_mod_family_missions_expaneded.gfx** file in the *interface* folder accordingly to your mod (aka replace the "missions" accordingly, e.g. with "subjects", "governments", "national_ideas", etc.).

**3.** Open that file and do the same for the entry. This will ensure that, if your mod is active, the icon with the green checkmark is shown for it.
  ```
  spriteTypes = {
	  # Mod Icon:
	  spriteType = {
		  name = "GFX_mod_icon_missions_expanded"
		  textureFile = "gfx/interface/expanded_mod_family/missions_expanded_icon_active.dds"
      }
  }
  ```

**4.** Open the **expanded_mod_family_l_english.yml** file in the *localisation* folder and copy the specific line of your mod, e.g. **MOD_TEXT_NATIONAL_IDEAS_EXPANDED: "§YNational Ideas Expanded§!"** for the *National Ideas Expanded* mod.

**5.** Rename the **\_expanded_mod_family_missions_expanded_l_english.yml** file in the *localisation/replace* folder accordingly to your mod (aka replace the "missions" accordingly, e.g. with "subjects", "governments", "national_ideas", etc.).

**6.** Open that file and replace the existing mod line with the copied line from step **4**.

 For example:
   ```
   l_english:
    MOD_TEXT_NATIONAL_IDEAS_EXPANDED: "§YNational Ideas Expanded§!"
   ```

**7.** Exchange the **§Y** in that line with **§G**.
   
 For example:
   ```
   l_english:
    MOD_TEXT_NATIONAL_IDEAS_EXPANDED: "§GNational Ideas Expanded§!"
   ```

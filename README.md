# Expanded Mod Family GUI
The files required for the GUI in the lobby that displays all Expanded Mods and which are active.

## How to update
The procedure is basically the same as for adding, however you require less steps. You do not have to copy the files again that are specifically for one mod, so **zzz_expanded_mod_family_missions_expanded.gfx** and **\_expanded_mod_family_missions_expanded_l_english.yml**. You do not have to do those steps again. Otherwise you just copy the other files over and overwrite/merge conflicting files.

## How to add
**1.** Copy all folders in your mod, overwrite files if needed (if you have an older version already in your mod, otherwise merge conflicting files).

**2.** Rename the **zzz_expanded_mod_family_missions_expanded.gfx** file in the *interface* folder accordingly to your mod (aka replace the "missions" accordingly, e.g. with "subjects", "governments", "national_ideas", etc.).

**3.** Open that file and do the same for the entry. **Note that there are two instances here that you have to change, in the *name* line and in the *textureFile* line.** This will ensure that the icon with the green checkmark is shown for your mod, when your mod is active.
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

**7.** Exchange the **§Y** in that line with **§G**. This will ensure that in the list the name of your mod is highlighted in green, when it is active.
   
 For example:
   ```
   l_english:
    MOD_TEXT_NATIONAL_IDEAS_EXPANDED: "§GNational Ideas Expanded§!"
   ```

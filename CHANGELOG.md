Any notable and major updates will be listed here going forward.

# Changelog

## Update #2 on Feb 10th (7 PM EST)

### Changed

* The template and blacklist jsons were moved to a json folder, and all of the log / A1111 / InvokeAI .txts to an outputs folder for organization, so the main folder isn't clogged up with random files.
* The code was restructured, with all of the heavy lifting done by the scripts in the scripts folder. The main UI script still starts and works the same. This was done in preparation for a future move to a new UI and adding new, advanced features.
* Settings file is deprecated for the time being.

## Update on Feb 10th

### Changed

* Prompts are now stored as lists in .txts. This means you can now add, remove, or relocate entire prompt lists extremely easily, as well as add prompts from existing lists, like [jumbo and devilkkw](https://github.com/adieyal/sd-dynamic-prompts/tree/main/collections)'s prompts for the Dynamic Prompts extension. The keywords still function the same. Simply type the filename of the .txt in brackets, without '.txt'.

### Added

* A script for exporting your existing dicts.py into .txts for use in the new structure, in case you modified it at all.

### Removed

* dicts.py as it won't be needed from now on.

### Fixes

N/A

## Update on Jan 31st

The below changes were made to `promptgen.py`.

### Changed

* Log.txt and log file in the UI box now read from newest to oldest.

### Added

* Added support for multiple generated prompts in one click for A1111 and Invoke outputs.
* Added support for being able to delete templates.json, blacklists.json, and the log.txt. This makes it easier to forego the default templates and blacklists to create your own without editing the .jsons.

### Removed

N/A

### Fixes

* Major performance fix for logging. When generating multiple-numerous prompts at once, the log would often only get a partial output. This is now fixed for logs.txt as well as the A1111 and Invoke logs. You should be able to generate dozens of prompts in one go without issue.

# MMI3G-GEM-Enable
Enable the Green Menu on Harman-Becker MMI3G infotainment systems.

As delivered from production, Harman-Becker MMI3G infotainment systems used in VAG cars do not have the so-called Green Engineering Menu (GEM) enabled.  This includes the RNS-850 used in Volkswagen Touareg models from 2011.

The GEM is often enabled as an adaptation to control module J794 at Address 5F using VAG aware diagnostic tools like VCDS, OBDeleven, and others.  When these tools are not available, the GEM can be enabled changing the persistent configuration appropriately.

The solution offered here uses binary sqlite3 to update the field that enables the GEM in file DataPST.db stored in persistent flash memory.  To enable the GEM, download the ZIP archive and extract to a blank FAT32 SD card directly.  Start the MMI system and wait for all functions to start fully.  Insert the SD card in an open slot and follow the displayed prompts.  After the script is complete, eject the SD card, review the saved plain-text log file saved to the SD card, and restart the MMI system manually.  The GEM will be enabled permanently following the next system restart.

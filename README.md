All the source code is written in the src folder (Main.java, PwConsole.java, PwInfo.java, and PwManager.java).
By the way, the AES-encryption function requires SunJCE to work, but SunJCE is probably included in the JDK already.


One sentence each on the purpose of each Java class in the src folder: 
-
• Main.java: contains the main-method, which contains the console.run() function that runs functions of the PwConsole class.

• PwConsole.java: outlines every function of the PwManager class that involves direct user-interaction (incl. load/search/add/edit/delete/save entries; gatekeeping the user from the program unless they know the correct master-password; changing the master-password).

• PwManager.java: has the core functions of the password manager, incl. encryption/decryption and file management; also uses contents of the PwInfo class to create an ArrayList called "pwInfoList" in which the user's entries are loaded.

• PwInfo.java: describes the variables/features of the pwInfoList ArrayList of the PwManager class; also includes getters and setters.



Thank you for your attention.
~ Seohyun

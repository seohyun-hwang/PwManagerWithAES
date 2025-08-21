All the source code is written in the `src` folder (`Main.java`, `PwConsole.java`, `PwInfo.java`, and `PwManager.java`).<br>
By the way, the encryption/decryption requires SunJCE to work, but SunJCE is probably included in the JDK already.


1-2 sentences each on the role of each Java class in the `src` folder: 
-
• <b>`Main.java`</b>: contains the main-method, which contains the `console.run()` function that runs functions of the `PwConsole` class.<br>
• <b>`PwConsole.java`</b>: outlines every function of the `PwManager` class that involves direct user-interaction (incl. load/search/add/edit/delete/save entries; gatekeeping the user from the program unless they know the correct master-password; changing the master-password).<br>
• <b>`PwManager.java`</b>: has the core functions of the password manager, incl. encryption/decryption and file management; also uses contents of the `PwInfo` class to create an ArrayList called "pwInfoList" in which the user's entries are loaded.<br>
• <b>`PwInfo.java`</b>: describes the variables/features of the pwInfoList ArrayList of the `PwManager` class; also includes getters and setters.<br>


Thank you for your attention.<br>
~ Seohyun

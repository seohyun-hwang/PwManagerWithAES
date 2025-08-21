Description: Password manager (load, search, add, edit, delete, save, save-and-quit) with AES encryption and OOP; the correct master password is required to gain entry into the manager.<br>

All the source code is written in the `src` folder (`Main.java`, `PwConsole.java`, `PwInfo.java`, `PwManager.java`).<br>
By the way, encryption/decryption requires SunJCE to work, but it's probably included in the JDK already.

How to use
-
1. Run the main-method
2. Press ENTER
3. Enjoy

1-2 sentences each on the role of each Java class in the `src` folder: 
-
• <b>`Main.java`</b>: contains the main-method, which contains the `console.run()` function that runs functions of the `PwConsole` class.<br>
• <b>`PwConsole.java`</b>: outlines every function of the `PwManager` class that involves direct user-interaction (incl. load/search/add/edit/delete/save entries; gatekeeping the user from the program unless they know the correct master-password; changing the master-password).<br>
• <b>`PwManager.java`</b>: has the core functions of the password manager, incl. encryption/decryption and file management; also uses contents of the `PwInfo` class to create an ArrayList called `pwInfoList` in which the user's entries are loaded.<br>
• <b>`PwInfo.java`</b>: describes the variables/features of the `pwInfoList` ArrayList of the `PwManager` class; also includes getters and setters.<br>

Encryption details
-
• <b>Provider of encryption</b>: SunJCE<br>
• <b>Method of encryption</b>: Advanced Encryption Standard (AES)<br>
• <b>Core encryption/decryption functions (all in `PwManager.java`)</b>: `getKeyFromPassword(String masterPw)`, `encryptObject(Serializable object, String masterPw)`, `decryptObject(SealedObject sealedObject, String masterPw)`<br>
• <b>Plain-text used to derive key</b>: master password<br>
• <b>Key length</b>: 256 bits<br>
• <b>Key-expansion iteration-count</b>: 256<br>
<br>

Thank you for your attention.<br>
~ Seohyun

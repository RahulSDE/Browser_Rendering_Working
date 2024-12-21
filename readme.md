## **How Browser Rendering Works**
- Browser is a simple software that can load some files from your computer(HDD/SSD) or it can load some files 
  from a remote (something which is not present with you) server.
                        |
                        |
    Then browser figures out how to display your content.

- **How Browser compute how to display any file??
    - Browsers have an engine that decides algorithmically how to display content.
    - `Browser engines:`  is a simple piece of software that understands what it can display and algorithmically decides how it can display.
        - Ex: Geko, Blink, Webkit.

### **HOW BROWSER LOADS THE FILES???**
- 
    ```
        html------->|--------------------
        css ------->|                   |
        javascript->|     BROWSER       |
                    |-------------------|
                                           -------------
                                           | Html file |
                                           -------------
                                               |
                 Browser read this html file   |
                 in the form of bytes          |
                                               |
                                  ------------------------------------
                                  | Bytes are converted to character |
                                  ------------------------------------
                                               |
                                Tokenization   | Tokenization means breaking string into multiple tokens using separator.   
                                using a parcer | In html file separator is <></>
                                               |  
                                  -------------------------------------  
                                  |  Browser converts token into nodes |
                                  --------------------------------------
                                               |
                Nodes is an object present     | Every nodes is considered distinct with distinct properties.
                stores in memeory              |
                                -------------------------------------------
                                |    Represent nodes in the form of tree.  |
                                --------------------------------------------
                                               |
                                               |
                                               |
                                 -------------------------------------   
                                 |   Dom tree (Document Object Model) |
                                 --------------------------------------
    ```


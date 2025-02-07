# Making all submenu entries show up

#### Corresponding branch: [remove_menu_arrows](https://github.com/Juliapixel/M3da/tree/remove_menu_arrows)

#### List of [changes](https://github.com/Juliapixel/M3da/compare/master...remove_menu_arrows)

-----

The file [`M3da/MainFrm.cpp`](/M3da/MainFrm.cpp) has all the keystroke handling logic. in it, the class method `CMainFrame::OnCreate` handles the creation of all elements on the main view, during the initialization of all elements on the window's main frame. On [line 353](/M3da/MainFrm.cpp#L353), the method called makes it so only "basic commands" are shown by default. Commenting out this line, by adding `//` to the start of it, disables this method call and makes all menu options show up.

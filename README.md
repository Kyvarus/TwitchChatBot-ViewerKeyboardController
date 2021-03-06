# TwitchChatBot-ViewerKeyboardController
Made to serve a custom twitch chatbot; mostly involving "Twitch Plays". This app can send customizable strings from any set key on your keyboard to your active textbox. These custom strings need to meet up with the channel bot's intended commands or they will be useless. 

"This program can be opened easily and does not require any prior setup."

The purpose of this application is simply to convert the duration of a key press from a user, into a string that contains the "Intended Context" and the Duration values.
Intended Context can vary largely, but generally this script will put out "!" before every command phrase.

You can set any normal key, to any ![phrase]. 
(This system was setup for JRPG games and uses the old PS1 controller sceme.) (left, right, up, down, cross, circle, triangle, square, etc.) All the actual names for these button-values have a hotkey bind menu; so you don't need to know them here.

PS1 Buttons that work with the chatbot are predefined and also hardcoded into the app; so you wont lose the defaults even if you delete your save.

There is two types of string-commands in this app, one is a duration based Button output ("![Button] [secs]" --> "!CROSS 5.2")
  This type can only be one of the predefined PS1 buttons that are in the defaults. 
The second type is a simple Keypush to send a string of text. (Pushed"hotkey")---->(Spits out "![command]")
  Both the Hotkey and the command argument are configurable when inside the app.
  
Predefined Actions for the PS1, (up, left, right, down, upleft, upright, downleft, downright) are able to produce "dash" commands by being pressed in caps-lock. This will send "![direction] [duration] dash" and cause your character to press the sprint command while inputting the direction. 
  
The way this app behaves is similar to that of a game controller. When you start the application in the main menu; your normal keyboard functions will be suppressed. But at any point in time you can quit out of the "gamepad mode" by hitting the "ESC" key.

Multi-Layout Support, with the ability to quickswap Layouts via hotkey! You can bind a specific layout to a hotkey and swap between it in the Controller Pause state. This will allow you to have an unlimited amount of phrases on a keyboard.

Using this technique, users are able to effectively use the custom Chatbot system and jump in and out of gameplay cleanly.
  
Recently Added:
- The ability to set duration output strings. 
- The ability to unset a specific duration output string without deleting the action. (You set the keybind to "NONE".)
- The ability to list Binds, Manuvers and combos from the settings menu.
  
  
Known Issues: 
- Currently only working on windows. 
- Cannot interpret numpad keys. ("NUM_4" for example will not do anything I found. IT hooks properly and blocks the key, but also doesn't do anything while pressed. Will investigate.)
- Conflicting Hotkeys will find issues getting both commands to come through.

# sologue
A one-node dialogue system for Godot 2.x

I have originally made this for a game of my own, given that I wanted to have something that wouldn't require any additional nodes to use. I tried out the two systems available for Godot at the AssetLib, but neither fit my needs. And so here we are, with this script.

Features capability for drawing text with effects, like *wave, bounce, shake* or even altering the delay, all inside one string.

I've distributed this code under the *MIT License*. I'd be happy to see contributions to make this system work even better or have my name be mentioned somewhere for the effort of making this.

###How to use
To set this up for use, you need to first attach this script to a Control node, such as NinePatchFrame or ColorFrame.  You also need to set up a font, prefferably a DynamicFont which allows changing sizes, which you then save as a resource file. That resource file is what you use inside the script for use.
To start a dialog, you use the **run_dialog()** method with an array holding the dialogue passed as a parameter. I've left out an example inside to show how that looks like.
To progress with the dialogue, you will have to set up an input process to handle that with the use of **next_line()**, and when the whole dialogue is done, a **dialog_end** signal is emitted.

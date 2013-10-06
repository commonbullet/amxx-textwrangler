# Amxmodx - TextWrangler / BBEdit


### Summary
This projects focus on providing tools in order to aid the development of AMX Mod X plugins on OSX with TextWrangler and BBEdit text editors.

TextWrangler is a light weight and free version of BBEdit (this one costs about $50). The scripts provided here is about the same, language code files are identical.
BBEdit is a more robust editor though, it includes an autocomplete feature (which's very helpful by the way), among other features.
You might want to check Barebones site to read the [full comparison](http://www.barebones.com/products/bbedit/comparison.html) of these products.

Currently, the tools provided here are:
* Compiling in these editors, with commands that may be accessed through editors menu or key binds (these keys must be configured on editor).
* Shortcut for opening amxmodx plugins.ini, the same way as above
* Highlights for pawn and Amx Mod X specific keywords. On BBEdit these keywords are used on autocomplete.

## Menu Scripts

### Features

* Menu scripts are written in AppleScript, allowing them to be called directly from TextWrangler/BBEdit menu.
* It takes advantage of the new Half-Life structure so it can check which mod has an amxmodx installation.
* If there's more than one mod with amxmodx, you might choose in which to compile from a list.
* Compiling output is straightforward, it goes to amxmodx/plugins.
* It does a fairly decent job on terminal tabs, creating new ones for new compilations and using the existing ones in case they are already there.

### Installation
1. Download the files from TextWrangler folder
2. Find the <code>TextWrangler/Scripts/AmxModx</code> or <code>BBEdit/Scripts/AmxModx</code> directory (depending on which editor you're installing) inside downloaded files
3. Open the <code>Scripts</code> folder inside <code>&lt;user home>/Library/ApplicationSupport/TextWrangler</code> or <code>&lt;user home>/Library/ApplicationSupport/BBEdit</code>. The easiest way to do that is to run TextWrangler/BBEdit, go to menu Scripts (that one with an icon ) >"Open Scripts Folder".
4. Drop the <code>AmxModx</code> folder from download inside <code>Scripts</code> you just opened.

### Language code definition for Pawn - AMXX

Yet to be written, but installation is almost the same as the compiling scripts, except that the content to be transfered should be that one inside <code>Language Code</code> folder.

## Known problems

### Menu Scripts
* There's a weird delay when compiling commands are called through editors, I couldn't figure out why it happens. When scripts are called directly through AppleScript Editor, there's no delay at all.

### Language Code
* Can't make the <code>^</code> character work as an escape in editor, even though I'm following Bare Bones [instructions](http://www.barebones.com/support/develop/clm.html) for building language code.

## Links
* [AMX Mod X site](http://www.amxmodx.org)
* [Bare Bones products page](http://www.barebones.com/products/)

## Credits
* Most keywords in for the language code were taken from [Arkshine](http://forums.alliedmods.net/member.php?u=7779)'s [Notepad++ definitions](http://forums.alliedmods.net/showthread.php?t=172128), which's also based on [fysiks](https://forums.alliedmods.net/member.php?u=30719)' [work](https://forums.alliedmods.net/showthread.php?t=86974).


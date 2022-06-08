# Section 1 - Setting Up a Local Development Environment (VSCode)

## Getting Started

First things first welcome to the first ever HubSpot Technical Consulting JavaScript Workshop 👋. Whether you are a JavaScript Newbie or a longtime JavaScript user this workshop has something for everyone. We decided to make this workshop self-paced as with our ever-changing schedules and customer requests it can be hard to find a time that works everyone 🙂. That said if you do find yourself struggling, have questions, or have feedback for improvements feel free to reach out to Sergio or Austin on the NAM Technical Consulting team. With that introductions done let's get into it and start by talking about Visual Studio Code (VSCode) and IDEs!

### What the heck is an IDE your title says VSCode?

That's a good question! An **IDE**, or **Integrated Development Environment**, is an application that enables developers to consolidate the different aspects of writing a computer program. IDE's increase programmer productivity by combining common activities of writing software into a single application just like HubSpot does for Marketers and Sales Reps in the CRM Space with all of our different Hubs 😏. Some of those activities include:

- Editing source code
- Building executables
- Debugging
- Etc.

**Well that's cool and all but we are not developers, so how does this help us?**

That's true! But just like developers we are always looking for ways to increase our productivity and consolidate the apps we use everyday. So let's talk about all the cool things we can get out of an IDE like VSCode (which will be the only IDE we talk about going further in this workshop).

### Syntax Highlighting

Based on the file extension (e.g. .json, .html, .js, etc.) of the file you are editing in VSCode (either natively or through an extension) knows the syntax of the file's language and can provide visual cues. Keywords are words that have special meaning like **class** in JavaScript and get highlighted in different color:

```
// Without syntax highlighting  
class Rectangle {  
    constructor(height, width) {
        this.height = height;
        this.width = width;
    }
}
```

```javascript
// With syntax highlighting
class Rectangle {
    constructor(height, width) {
        this.height = height;
        this.width = width;
    }
}
```

### Autocomplete

When VSCode knows your programming language, it can anticipate what you're going to type next!  

![Gif of VSCode Autocomplete](https://code.visualstudio.com/assets/docs/editor/intellisense/intellisense.gif)

### Debugging

Everyone makes mistakes 🤷  but how do know when we do And how do we fix them? Well VSCode has lots of debugging and even parses your code for error before it even runs.

![Gif of VSCode Error Parsing](https://code.visualstudio.com/assets/docs/nodejs/extensions/eslint.gif)

### Okay you sold me! Now how do I set this up?

## Setting Up VSCode Efficiently

Well the first step is to download VSCode onto your machine (don't worry it works on both Macs 🍎 and Windows 🪟, and Linux if you somehow have that on your work computer 🤷). You can download VSCode for your corresponding OS from this link [here](https://code.visualstudio.com/download).

Once your done with that you are pretty much ready to go for most of your daily use cases. But since we are Technical Consultants and always looking for the fastest and easiest way of doing things lets now customize some of the settings in VSCode to really increase our productivity.

### 'settings.json'

In VSCode all of your settings both native and extension specific (don't worry we will talk about extensions soon) live in the settings.js file. This file is located in the root of your VSCode installation folder. You can also access it by using the **Command Palette** which you can access on Mac by using `shift` + `⌘` + `p` and on Windows by using `Ctrl` + `Shift` + `p` and then typing in 'open settings' + `Enter`.

![Image of VSCode settings.json](https://code.visualstudio.com/assets/docs/getstarted/settings/lang-based-settings.png)

If you are not familiar with JSON, this can look pretty intimidating. But the good news is that you can also use the settings GUI to set the settings for both native and extension specific settings. You can access the settings GUI by clicking on the gear icon on the bottom right of the VSCode window.

### Recommended Settings

Now that we know how to get to the VSCode settings we can start adding some settings to help with our productivity and make it even easier to use VSCode.

#### Files

Files: Auto Save: onFocusChange - In my VSCode environment I have my setting Auto Save set to onFocusChange. This means that every time I switch tabs or move focus to another window VSCode will save my files. This is super helpful when working on multiple files at once (or if you are easily distracted by client emails and forget to save your work...repeatedly 😬)

#### Editor

Editor: Bracket Pair Colorizer: Enabled - This is a great feature that used to need an extension to work but is now supported natively in VSCode. It will highlight matching brackets when you are typing. This can be super helpful when you are trying to troubleshoot deeply nested JSON objects and ensure they are all closed properly.

Editor: Format On Paste: Enabled - One of my biggest gripes with the CMS Hub Editor is the lack of formatting tools and is such a pain to manually format big files. With VSCode we have access to extension like Prettier that we can set as out default formatter for our files. Then with this setting every time I paste something in my editor Prettier will automatically format it for me.

Editor: Format On Save: Enabled - This pretty similar to that first recommended setting where on saving of a file it will format my files. This is just nice because it saves you from having to go back and fix any messy code you created while writing your code.

Editor: Inline Suggest: Enabled - I actually thought this was enabled by default but according to my VSCode environment I modified it but I would recommend enabling it to ensure you get inline suggestions on your code.

Editor: Auto Close Bracket

#### JavaScript

JavaScript: Update Import On File Move: Enabled - Personally I hate having to go back and update file import paths when I move files around in a project. This setting automatically sets the paths for you when you move a file instead of you having to have to go redo all of your imports.

### Extensions/Themes

We all like a little customization from time to time. So let's dive into extensions and themes and see how they can make our time with VSCode even more enjoyable and productive.

#### Themes

Lets start with themes in VSCode since they are not a necessity for maximizing VSCode but can help make things more visually appealing and sometimes easier to read. To install a theme you can open up the extensions page by clicking the extensions icon in the left sidebar (or by using `shift` + `⌘` + `x` on Mac and `Ctrl` + `Shift` + `x` on Windows) and then searching themes in search box.
My personal goto theme is [SynthWave '84 by Robb Owen](https://marketplace.visualstudio.com/items?itemName=RobbOwen.synthwave-vscode) because I like the colors it uses plus the fact that you can make the background of text glow. But feel free to find a theme that works for you. In addition to the changing VSCode color scheme you can also change the icons that are used in the VSCode window. My go to icon theme is the [Material Icons pack by Philipp Kief](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) but if this doesn't work for you just like the SynthWave theme you can find a icon pack/theme that works for you or even better [make your own](https://docs.microsoft.com/en-us/shows/vs-code-livestreams/build-your-own-vs-code-theme)! 😎

#### Extensions

Okay so we now have our VSCode environment looking good but what about productivity? Well lets start by talking about how do we add an extension to VSCode. To install an extension it is the exact same as installing a theme or an icon pack. You find an extension by searching in the extensions page, click into the extension and then click the install button. Super easy right? Once you have installed the extension it will immediately start working but if you want uninstall it you can do so by going back to the extension's page in VSCode and clicking the uninstall button and if the extension supports extra settings you can find them in your VSCode settings.

###### Recommended Extensions

Here is a list of some of my goto extensions in VSCode and brief descriptions of what they do:

[:emojisense:](https://marketplace.visualstudio.com/items?itemName=bierner.emojisense) by Matt Bierner - I found adding emojis to documents such as this can be a pain with Apple's emoji keyboard but with this extension all I have to do is either add a : and then start typing the name of the emoji to add one or hit `⌘` + `i` and then select the emoji I want from the picker 🚀

![Gif of Emojisense](https://raw.githubusercontent.com/mattbierner/vscode-emojisense/master/media/example.gif)

[Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) by Jun Han - This extension will automatically close tags when you type a closing tag.

![Gif of Auto Close Tag](https://github.com/formulahendry/vscode-auto-close-tag/raw/HEAD/images/usage.gif)

[Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) by Jun Han - This extension will automatically rename

# Section 1 - Setting Up a Local Dev Environment (VS Code)

## Getting Started

First things first welcome to the first ever HubSpot Technical Consulting JavaScript Workshop 👋 . Whether you are a JavaScript Newbie or a longtime JavaScript user this workshop has something for everyone. We decided to make this workshop self-paced as with our ever-changing schedules and customer requests it can be hard to find a time that works everyone 🙂 . That said if you do find yourself struggling, have questions, or have feedback for improvements feel free to reach out to Sergio or Austin on the NAM Technical Consulting team. With introductions done let's get into it and start by talking about VSCode and IDEs!

### What the heck is an IDE your title says VSCode?

That's a good question! An **IDE**, or **Integrated Development Environment**, is an application that enables developers to consolidate the different aspects of writing a computer program. IDE's increase programmer productivity by combining common activities of writing software into a single application just like HubSpot does for Marketers and Sales Reps in the CRM Space with all of our different Hubs 😏 . Some of those activities include:

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

![Gif of VSCode Autocomplete]()

### Debugging

Everyone makes mistakes 🤷  but how do know when we do And how do we fix them?

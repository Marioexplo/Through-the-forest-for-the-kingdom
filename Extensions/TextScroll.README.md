### Description

Load a string or an array or structure of strings and start scrolling. Perfect for any kind of narrative scene.

### How to use the extension

### Common functions

- **Load** action: Load one or more strings. If you choose: String: put a text; Array: put a JSON (use ToJSON) which returns an array variable; Structure: put a JSON (use ToJSON) which returns a structure variable.
- **Start scrolling** action: start scrolling at a given timer and you can also do a firs scroll. If you use the _structure_ type, always give the branch name before scrolling by using the "structure string" action.
- **Scroll once** action: scroll just one letter.
- **Current text** expression: use it with text action of a text object to have a typewriter effect.
- **Restart** action: it will restart the scrolled letters' count and the internal timer.
- **End string** action: finish scrolling the current string.
- **Scrolling completed** condition: check if the current string has finished scrolling.
- **Is scrolling** condition: check if the extension is currently scrolling

### Array functions

- **Array number** expression/action: get/set the given array's number. This number is equal to the number of the child (so the first one is number 0).
- **Auto Array** action: enable a function to automatically switch from the string to the following one after a given time. Set the time to -1 to disable the function.
- **Strings finished** condition. check if the last string of an array has finished scrolling. Useful when used with the "Auto Array" function.

### Structure functions

- **Structure string** expression/action: get/set the given structure's branch name.

### Tips
Strings can be used for very short texts like instruction. Arrays are useful for interlude scenes, where the player just watch the dialogues. Instead, structures, can be used for interactive scenes.
### Description

This extension was initially created as an alternative for the "panel sprite button" object.
This extension contains:
-A behaviour for sprites to change animations when hovered/pressed
-A behaviour for texts to enable the outline and/or the shadow when hovered/pressed
-A behaviour for sprites to enable an effect and/or change one of its properties when hovered/pressed
-An object (advanced) with a sprite which changes animation when hovered/pressed and a BBtext over it

### How to use the extension

**For each behaviour**: you can decide wether to apply changes when the button is hovered, pressed or both. So, you'll always found a property, a condition and an action for these. Also, there is condition for when the button is hovered, and another one when it's pressed

- **Sprite Button** behaviour: for this behaviour to work, you'll need an animation named "Idle"; and if you check their respective, an animation named "Hovered" and another one named "Pressed"
- **Text Button** behaviour: on this behaviour you will find 2 other properties, conditions and actions: one to activate the outline and the other one to activate the shadow, when the text is hovered or pressed (as decided before)
- **Effect Button** behaviour: this behaviour works only with sprites and you'll have to have set at least one effect. 
You'll find a property where you have to put the name of the effect, and you'll also find an expression and an action for this.
Then there is a property to choose wether to enable the effect when the changes are applied, there is also a condition and an action.
If you want to change an effect's property's value, you'll have to put its name in the behaviour's property; if you don't want this, just leave it blank; then you have to declare if the given property is a number using a checkbox (if it isn't, then it assumes it's a color), there is also a condition for this and there is an expression which gives you the property's name, and an action where you have to specify if the property is a number or a color type.
Then, always if you want the effect's property to be changed, you have to give two numbers or colors: one for the original value and one with the modified one; for each type, there is also an expression and an action.

- **Button** object (advanced): the object works as the Sprite Button behaviour but it has also a BBtext object over it, for this reason there are two more expressions and actions: one for the text and one for the font size.
Because object are probably not intended to be used like this, there are some defects: first of all, in the editor the sprite's mask (which is used in the editor to select or move the instance) is always 64x64, even if the sprite is bigger or smaller; second thing, because of the previous issue and to make everything work, the BBtext can't be seen in the editor, but it's created with the object or at the start of the scene. In practice everything works, but you should have in mind these defects before working with the object, and if you don't need to have a text over the button, I suggest to use the Sprite Button behaviour.
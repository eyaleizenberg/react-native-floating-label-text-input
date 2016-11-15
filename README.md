## React Native Floating Label Text Input

### What is this?
This component will render an iOS styled text field with floating label animation. When there is no value, the placeholder will be centered. Once there is a value, the value will slide down and the label will fade in and slide up.

Credits for the concept to Matt D. Smith ([@mds](http://www.twitter.com/mds)), and his [original design](http://dribbble.com/shots/1254439--GIF-Mobile-Form-Interaction?list=users).

<p align="center">
    <img src ="http://i.imgur.com/5dddNix.gif" />
</p>

### Installation
```npm install react-native-floating-label-text-input --save```

### Usage example

```javascript
import FloatLabelTextInput from 'react-native-floating-label-text-input';

class SomeComponent extends Component {
  render () {
    return (
      <View>
        <FloatLabelTextInput
          placeholder={"name of field"}
          value={"value of field"}
          onFocus={@myFocusFunction}
          onBlur={@onBlurFunction}
        />
      </View>
    );
  }
}
```

### Component props
- placeholder (String) - String that will be used as the placeholder if there is no value. It will also be the string used for the label when there is a value.
- secureTextEntry (Bool) - If true, the text input obscures the text entered so that sensitive text like passwords stay secure. The default value is false.
- keyboardType (Enum) - enum('default', 'email-address', 'numeric', 'phone-pad', 'ascii-capable', 'numbers-and-punctuation', 'url', 'number-pad', 'name-phone-pad', 'decimal-pad', 'twitter', 'web-search').
- value (String) - Value of the text input.
- onFocus (Function) - Function to be called on focus.
- onBlur (Function) - Function to be called on blur.
- onChangeTextValue (Function) - Function to be called when text is modified.
- noBorder (Boolean) - Hide the border bottom of the field.
- maxLength (Number) - Limits the maximum number of characters that can be entered. Use this instead of implementing the logic in JS to avoid flicker.
- selectionColor (String) - The highlight (and cursor on ios) color of the text input.

### Questions/Bugs/Ideas?
Feel free to open an issue on github, send suggestions, fork this repository or contact me at eyal.eizenberg@samanage.com

This package was developed during my work at [Samanage](http://www.samanage.com/).

Thanks and Enjoy! :)

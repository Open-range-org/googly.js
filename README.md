# Googly.js
[![Build Status](https://travis-ci.com/NIHAR-SARKAR/Matroska.svg?branch=master)](https://travis-ci.com/NIHAR-SARKAR/Matroska)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/NIHAR-SARKAR/Matroska/blob/master/LICENSE)

"Googly.js is a lightweight JavaScript validation library. If you’re unfamiliar with handling validation in JavaScript or if you’re looking for a library to assist with validation, Googly.js is a great choice.

## Valid Tag

### validate Required field
To perform required validation, use the `valid` tag with the `type` attribute set to `require`

Map the `for` attribute to the corresponding text input field by setting its value to the same ID as the text input field.

Customize the validation message by specifying the desired content for the `message` attribute.

If you want to style the custom message with a specific color, apply your custom CSS class. For instance, if you’re using the Bootstrap CSS library and want a red-colored message, use the “text-danger” class.


```html
<input type="text" placeholder="Enter Id Number" id="idnum" class="form-control" />
<valid type="require" for="idnum" msg="Please insert Id number" class="text-danger"></valid>

```

### validate expression field
To perform expression validation, use the `valid` tag with the `type` attribute set to `expression`

Map the `for` attribute to the corresponding text input field by setting its value to the same ID as the text input field.

Customize the validation message by specifying the desired content for the `message` attribute.

`mode` attribute helps to check expression . need to mention what type of expression you want to validate . 4 options available :
- `num`  : Only numbers are allowed
- `char` : Only characters are allowed"
- `pass` : Only Number and Characters are allowed
- `mail` : o=Only valid email pattern allowed

If you want to style the custom message with a specific color, apply your custom CSS class. For instance, if you’re using the Bootstrap CSS library and want a red-colored message, use the “text-danger” class."


```html
<input type="text" placeholder="Enter Firstname" id="fname" class="form-control" />
 <valid type="expression" for="fname" mode="char" msg="Only characters are allowed" class="text-danger"> </valid>

```

### remain field
To limit the maximum character count for a field and display the remaining characters to be typed, you can utilize the “remain” attribute.

Add the “maxlength” attribute to the input field. Set its value to a numeric limit representing the maximum allowed characters.

To perform character remain calculation , use the `valid` tag with the `type` attribute set to `remain`

Map the `for` attribute to the corresponding text input field by setting its value to the same ID as the text input field.

If you want to style the custom message with a specific colour, apply your custom CSS class. For instance, if you’re using the Bootstrap CSS library and want a red-colored message, use the “text-danger” class.


```html
<textarea class="form-control" rows="10" cols="30" maxlength="250" data-validation="remain" id="textarea"></textarea>
<valid type="remain" for="textarea" class="text-info"></valid>

```

### compare Required field
To compare values between two input fields, use the following validator:

Add the `valid` tag to the input field where you want to perform the comparison. Set the type attribute to `compare`.

Map the `for` attribute of the validator to the corresponding text input field by setting its value to the same ID as the text input field you want to compare (let’s call this (1)).

Map the `with` attribute of the validator to the other text input field by setting its value to the same ID as the second text input field (let’s call this (2)).

If the values of (1) and (2) don’t match, an error message saying `Mismatch!` will be displayed. 

```html
<input type="password" placeholder="Enter Pass" id="pass" class="form-control" />
<input type="password" placeholder="Confirm Pass" id="confpass" class="form-control" />
<valid type="compare" for="confpass" with="pass"></valid>

```

## strength Tag
To assess password strength and complexity, you can utilize the strength tag. This tag validates the following criteria:

- Lowercase characters
- Uppercase characters
- Special characters
- Numbers
Additionally, it considers the total length of the password. 

Map the `for` attribute to the corresponding input field by setting its value to the same ID as the text input field.

```html
<input type="password" placeholder="Enter Pass" id="pass" class="form-control" />
<strength for="pass"></strength>
```


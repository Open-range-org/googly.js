# Matroska
[![Build Status](https://travis-ci.com/NIHAR-SARKAR/Matroska.svg?branch=master)](https://travis-ci.com/NIHAR-SARKAR/Matroska)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/NIHAR-SARKAR/Matroska/blob/master/LICENSE)

"Googly.js is a lightweight JavaScript validation library. If you’re unfamiliar with handling validation in JavaScript or if you’re looking for a library to assist with validation, Googly.js is a great choice.

## Valid Tag

### validate Required field
To perform required validation, use the `valid` tag with the `type` attribute set to `require`

Map the `for` attribute to the corresponding text input field by setting its value to the same ID as the text input field.

Customize the validation message by specifying the desired content for the `message` attribute.

If you want to style the custom message with a specific color, apply your custom CSS class. For instance, if you’re using the Bootstrap CSS library and want a red-colored message, use the “text-danger” class."


```html
<input type="text" placeholder="Enter Id Number" id="idnum" class="form-control" />
<valid type="require" for="idnum" msg="Please insert Id number" class="text-danger"></valid>


```


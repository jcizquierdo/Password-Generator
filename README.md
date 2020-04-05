# Password-Generator

### I completed this Password Generator by using checkboxes instead of prompts. I thought it would be easier for the user to interact with the website.

I started by creating the Generator Functions using CharCode to get random lower and upper cases and random numbers and symbols.

Then I created variable elements to equal(=) to a document.getElementByID() that's in the HTML. 

To generate the event listen for the chackboxes and length value I included variables 
length, hasLower, hasUpper, hasNumber, and hasSymbol.

I also created a function named generatePassword to call the variables "lower, upper, number, symbols, and length" into my final generatedPassword.

To filter out unchecked boxes, which would have a boolean answer of "false" I used a typesArr with (item => Object.values(item)[0] to not include unchecked boxes in our generated password.

To loop using the length value I used a for loop. (for (let i = 0; i < length; i += typesCount)

Then to get the generatedPassword in the box I called on resultEl.innerHTML = finalPassword to get the generated password.

# DOM and JavaScript Practice
We will practice using JavaScript to manipulate the DOM of a webpage.

## Practice 1
1. All code for this problem will be completed in the `addH1HeadingElement()` function in `script.js`.
2. Utilizing the `document` object, create a new `h1` element by using the `createElement()` function and assign it to a variable.
3. Set the `textContent` property value of the `h1` variable to the string `"JavaScript Today"`.
4. Utilizing the `document` object and the `getElementById()` function, get the element whose id is set to `body` and assign it to a variable.
5. Call the `prepend()` function of the `body` variable and pass it the `h1` variable.  
  *Example:* `myElement.prepend(newElement);`
6. Run the code and you should see the `h1` is now displayed on the page.

How the web page looks after Practice 1:
![image](assets/image_2.png)

## Practice 2
1. All code for this problem will be completed in the `colorizeLoopNameHeaders()` function in `script.js`.
2. Utilizing the `document` object, get all elements that have the class name `codeFont` by using the `getElementsByClassName()` function and assign the array of elements to a variable.
3. Create a `while` loop that has its condition set to a count that starts at zero and keep going while the loop count variable is less than the length of your variable, increment the variable by one for each iteration at the end of the loop.
4. Inside the loop use the loop count variable to get element at that index of your array and use the `classList` property on the variable to call the `add` function and pass it the value `"codeColor".  
  *Example:* `myArray[myIndex].classList.add("CssClass");`
5. Run the code and you should see the `for`, `while`, and `do/while` text colored blue in the article titles.

How the web page looks after Practice 2:
![image](assets/image_3.png)

## Practice 3
1. All code for this problem will be completed in the `addFlexLayout()` function in `script.js`.
2. Utilizing the `document` object, get all elements with the tag `div` by using the function `getElementsByTagName()` and assign the array of elements to a variable.
3. Create a variable that will be used as the index of the array and initialize it to zero.
4. Create a `while` loop whose condition is to make sure that the index variable is less than the length of your array of `div` elements.  This loop will iterate over the divs array.
   1. Inside the while loop you should use the `add()` function on the `classList` property available on each `div` element in the array and pass in the CSS class name string `"flexContainer"` to the `add()` function.  
    *Example:* `myArray[myIndex].classList.add("CssClass");`
   2. Increment your index variable by one
   3. That is all that will be done inside the `while` loop
5. Utilizing the `document` object, get all elements with the tag `article` and assign the array of elements to a variable.
6. Set your index variable used in the `while` loop above to zero.
7. Create a `do/while` loop, this loop will iterate over the articles array.
   1. For the condition of the while loop, have it make sure that the index variable is less than the length of the articles array created in step 5.
   2. Inside the `do/while` loop, use the `classList` property and it's `add()` function to add the CSS class name `"flexItem"` to each of the `article` elements in the array.  
    *Example:* `myArray[myIndex].classList.add("CssClass");`
   3. Increment the index variable by one.
8. Run the code, you should see that the articles are no longer in one column but instead in two rows.

How the web page looks after Practice 3:
![image](assets/image_4.png)

## Practice 4
1. All code for this problem will be completed in the `styleArticles()` function in `script.js`.
2. Utilizing the `document` object, get all elements with the tag `article` and assign the array of elements to a variable.
3. Create a `while` loop that has its conditional statement set to a count that starts at zero and keep going while the loop count variable is less than the length of the `article` array, increment the variable by one at the end of the loop.
4. Inside the `while` loop do the following:
   1. Use the `classList` property and it's `add()` function to add the CSS class `"articleShadow"` to each of the `article` elements in the array. 
    *Example:* `myArray[myIndex].classList.add("CssClass")'`
   2. Use the `classList` property and it's `add()` function to add the CSS class `"roundedBorder"` to each of the `article` elements in the array.
   3. On each of the articles, use the `firstElementChild` property and use the `add()` function on it's `classList` property to add the CSS class `"articleTitle"`.  This will grab the first child element in the `article` element, which should be the `h2` element and add the CSS class to it.
    *Example:*  `myArray[myIndex].firstElementChild.classList.add("CssClass");`
5. Run the code, you should see rounded borders, shadows, and background color on the article titles.
   
How the web page looks after Practice 4:
![image](assets/image_5.png)

## References
* [Arrays](https://www.w3schools.com/js/js_arrays.asp)
* [createElement()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement)
* [getElementsByClassName()](https://www.w3schools.com/jsref/met_document_getelementsbyclassname.asp)
* [getElementById()](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById)
* [getElementsByTagName()](https://www.w3schools.com/jsref/met_document_getelementsbytagname.asp)
* [prepend()](https://developer.mozilla.org/en-US/docs/Web/API/Element/prepend)
* [while and do/while loops](https://www.w3schools.com/js/js_loop_while.asp)

## Configuration

### GitDoc

GitDoc is a great extension to automatically commit and push changes into the repository. For developers who are just getting started with web development, configuring this extension to automatically save their changes can make the introduction into git version control a much less intimidating experience. Because the extension cannot be configured by default to automatically push the changes up to the repository, users will need to update the settings the first time they launch project in Codespaces.

1. On the right-hand side of the `Codespaces` editor, click on the `Extensions` icon.

![image](.assets/extensionIcon.jpg) 

2. Once the `Extensions` sidebar expands, click on the gear icon in the `GitDoc` extension card and then select `Extension Settings` from the menu.

![image](.assets/extensionSettingClick.jpg)

3. Update the `Auto Commit Delay` to the number of milliseconds you would like the plugin wait before checking for file changes. The number is in milliseconds, 1 second = 1000 milliseconds. I've found the 5000 is a good number to use.

![image](.assets/autoCommitDelay.jpg) 

4. (Optional) Change the `Commit Validation Level` to `none`. This will allow all changes, even those that might include code which has errors in it, to be saved.

![image](.assets/commitValidation.jpg) 

5. Check the box associated with `Enabled` under the `Commit Validation Level` section.

6. Refresh the page in your browser so that the settings can be applied to the editor.

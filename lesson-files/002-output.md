# JavaScript Output

JavaScript can "display" output in 4 simple and different ways:

1. Using `innerHTML` property.
2. Using `document.write()` method.
3. Using `Alert` box
4. By logging on the `console`.

## Using innerHTML property.

`innerHTML` Give you the abibility to set or get the `HTML` markup contained within the element  

```javascript
// Set or update the contents of an element
document.querySelector("h1").innerHTML =
   "Hello <span style='color:red;'>World</span>";

// Reading the HTML contents of an element
let content = document.querySelector("h1").innerHTML;
```

It is not uncommon to see innerHTML used to insert text into a web page. There is potential for this to become an attack vector on a site, creating a potential security risk. 

## Using document.write() method

The **document.write()** method writes a string of text to a document stream.  

**Syntax:**  

markup parameter is a string containing the text to be written to the document.  

```javascript
   write( markup );
```

**Example:**  

```javascript
   document.write( "<span style='color:red'>Hello javascript</span>" );
```

**Note:** This method has very idiosyncratic behavior. In some cases, this method can affect the state of the HTML parser.  
The developers recommend to avoid using document.write().

## Using Alert box

instructs the browser to display a dialog with an optional message, and to wait until the user dismisses the dialog.  

**Syntax:**  

message parameter is a string you want to display in the alert dialog

```javascript
   alert( message );
```

**Example:**   

```javascript
   window.alert( "Hello visitor" );
```

Alert boxes are modal windows they prevent the user from accessing the rest of the program's interface until the dialog box is closed. For this reason, you should not overuse any function that creates a dialog box (or modal window).

## logging on the console.

The console.log() method outputs a message to the web console.  
The message may be a single string (with optional substitution values), or it may be any one or more JavaScript objects.

**Syntax:**  

**msg** is a JavaScript string containing zero or more substitution strings.  
**obj** is a list of JavaScript objects to output

```javascript
   console.log( msg );
   console.log( msg, msg2 );
   console.log( obj );
```

**Example:**   

```javascript
   console.log( "Hello from console" );
   console.log( 5 + 5 );
```
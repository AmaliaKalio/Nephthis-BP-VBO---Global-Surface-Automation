# Nephthis-BP-VBO---Global-Surface-Automation
VB Library intended to replace certain core functionality of BP Surface Automation tools in a significantly quicker and more efficient manner

## Click Image Center
Clicks the specified image in the center

### Inputs:
* Image - Image
* Tolerance - Text
* Mouse Button - Text

## Click Image Offset
Finds an image and clicks an offset amount of pixels away from it

### Inputs:
* Image - Image
* Tolerance - Text
* Mouse Button - Text
* Offset Anchor - Text
* Offset X - Number
* Offset Y - Number

## Create Tolerance (Absolute)
Returns a specially-constructed tolerance string to be used by other pages for image comparisons. Each color component is specified as an absolute number indicating how much tolerance should be allowed. A tolerance of 8 means a color value of 100 will match a color value of 92.

### Inputs:
* Red Tolerance - Number
* Green Tolerance - Number
* Blue Tolerance - Number

### Outputs:
* Tolerance String - Text

## Create Tolerance (Absolute)
Returns a specially-constructed tolerance string to be used by other pages for image comparisons. Each color component is specified as a percentage indicating how much tolerance should be allowed. A 10% tolerance means a color value of 225 will match a color value of 200.

### Inputs:
* Red Tolerance - Number
* Green Tolerance - Number
* Blue Tolerance - Number

### Outputs:
* Tolerance String - Text

## Find Image
Finds the specified image using the specific color tolerance and returns the top-left coordinates

### Inputs:
* Image - Image
* Tolerance - Text

### Outputs:
* Contains - Flag
* X Index - Number
* Y Index - Number

## Wait for Image Appearance
Waits either for the specified image to appear, or for the specified timeout to occur, then returns the coordinates if found.

### Inputs:
* Image - Image
* Tolerance - Text
* Max Wait - Number

### Outputs:
* Contains - Flag
* X Index - Number
* Y Index - Number

## Wait for Image Disappearance
Waits for the specified image to disappear from the screen

### Inputs:
* Image - Image
* Tolerance - Text
* Max Wait - Number

### Outputs:
* Disappeared - Flag

## Move Mouse (fast)
Jumps the mouse to the specified screen coordinates

### Inputs:
* Coord X - Number
* Coord Y - Number

## Move Mouse (tweened)
Simulated mouse movements to move the mouse to the specified coordinates. Moves across X, then across Y.

### Inputs:
* Coord X - Number
* Coord Y - Number

## Move Mouse (tweened with wait)
Simulated mouse movements to move the mouse to the specified coordinates. Moves across X, then across Y. Additional input to allow delay time between coordinate steps, in decimal format.

### Inputs:
* Coord X - Number
* Coord Y - Number
* stepInterval - Number

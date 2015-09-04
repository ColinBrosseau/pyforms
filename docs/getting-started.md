# Getting started

This page was based in the examples available on the github folder: [Tutorial - SimpleExamples](https://github.com/UmSenhorQualquer/pyforms/tree/master/tutorials/1.SimpleExamples)


## **Prepare the application class**
***************************

1. Create the Python file that will store your applications. Example: SimpleExample.py
2. After import pyforms, the BaseWidget and Controls classes you will need:
```python
import pyforms
from   pyforms 			import BaseWidget
from   pyforms.Controls import ControlText
from   pyforms.Controls import ControlButton
```
3. Create your application class. This class should inherit from the class BaseWidget.
```python
class SimpleExample1(BaseWidget):
	
	def __init__(self):
		super(SimpleExample1,self).__init__('Simple example 1')

		#Definition of the forms fields
		self._firstname 	= ControlText('First name', 'Default value')
		self._middlename 	= ControlText('Middle name')
		self._lastname 		= ControlText('Lastname name')
		self._fullname 		= ControlText('Full name')
		self._button 		= ControlButton('Press this button')

##################################################################################################################
##################################################################################################################
##################################################################################################################

#Execute the application
if __name__ == "__main__":	 pyforms.startApp( SimpleExample1 )
```


## Example 1

Shows the most simple way to create windows forms application using 

![Simple example ](SimpleExample1/screenshot.png?raw=true "Screen")



## Example 2

Shows you how to organize the forms using the variable "self._formset".

![Simple example ](SimpleExample2/screenshot.png?raw=true "Screen")



## Example 3

Shows you how to organize the forms **side by side** using the variable "self._formset".

![Simple example ](SimpleExample3/screenshot.png?raw=true "Screen")



## Example 4

Shows you how to **define tabs** using dictionaries in the variable "self._formset".

![Simple example ](SimpleExample4/screenshot.png?raw=true "Screen")



## Example 5

Shows you how to define the **application main menu** using the BaseWidget.mainmenu property.

![Simple example ](SimpleExample5/screenshot.png?raw=true "Screen")



## Example 6

This example shows you how to implement a **popup menu** for a Control.

![Simple example ](SimpleExample6/screenshot.png?raw=true "Screen")
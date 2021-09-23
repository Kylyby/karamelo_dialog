# karamelo_dialog
## Karamelo helps you easily create a selection menu that doesn’t require the user to manually type in the option they want to choose 
### How to install:

In the terminal/shell, type in:

```
pip install karamelo
```
  
### How to use:
  
begin by importing the package:
  
```py
import karamelo
```
  
Then set a variable and call the function in it:
```py
karamelorun = karamelo.dialog()
```
  
inside the function we have 3 parameters: background color of the selection(bgcolor), number of options that can be selected(limit) and the options(options). bgcolor must be a string, limit an integer and options a list
  
  Example:
  
```py
karamelorun = karamelo.dialog(bgcolor='red', limit=4, options=['one', 'two', 'three', 'four'])
```

  colors accepted for bgcolor:
  
```py
'black'
'red'
'green'
'yellow'
'blue'
'purple'
'cyan'
```

At the end, the variable set above will return a value, you can use this value to define what each option does. This value always starts on 0, so the value of the option is gonna be the value of it's position -1, for example: the 3rd option is gonna have the value of 2
  
use demonstration:

```py
if karamelorun == 0:
  print('pineapple')
elif karamelorun == 1:
  print('banana')
elif karamelorun == 2:
  print('apple')
elif karamelorun == 3:
  print('grape')
```
  
at the end of this demonstration we have the following code:
  
```py
import karamelo

karamelorun = karamelo.dialog(bgcolor='red', limit=4, options=['one', 'two', 'three', 'four'])

if karamelorun == 0:
  print('pineapple')
elif karamelorun == 1:
  print('banana')
elif karamelorun == 2:
  print('apple')
elif karamelorun == 3:
  print('grape')
```
#### Output of each option:

![image](https://user-images.githubusercontent.com/91160942/134447080-116d3050-476b-46fb-b285-f1dffbc8735d.png)     ![image](https://user-images.githubusercontent.com/91160942/134447164-c0fc24ac-bd46-402a-a800-80cd535ec055.png)

![image](https://user-images.githubusercontent.com/91160942/134447188-71053ed2-513e-4e8e-991e-bf39003368d7.png)     ![image](https://user-images.githubusercontent.com/91160942/134447236-b733ef4c-3b9e-4b2e-b334-6dce533d20af.png)


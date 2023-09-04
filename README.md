s# pci_ad23
Repo para almacenar los ejercicios y ejemplos de clase de "Pensamiento Computacional para Ingeniería". Semestre AD23

# TC1028.411 Project from Juan Pablo Ramos.

For the final delivery, the style of the PEP8 standard and convention will be applied to this project, as well as good industry practices seen throughout the course.

In the comments within each function, in parentheses, are the sub-competencies that that function or set of functions demonstrates.

# [](https://github.com/JuanPablo0947/pci_ad23#diario-nutricional)Nutritional Intelligent Diary

### [](https://github.com/JuanPablo0947/pci_ad23#contexto)[](https://github.com/JuanPablo0947/pci_ad23#contexto)Context

This program is keep track of my progress in the LiFE nutrition course with code KWEL3012. In fact, the program's objective is to lead the user know how their emotions affect the integral nutrition (i.e., sleep, hygiene, food, mental health, etc.) by collecting a series of information like the following:

- Emotions you got throughout the day
- food consumption
- hours of sleep (TBD)
- free information (whatever you want to add!)
- Body measurements
- Physical activity habits
- Between others...

Little by little by analyzing intricately each report generated by the program throughout your prolonged use, you will realize that there are patterns or relationships between what you eat and how you feel.

We recommend that when you are asked about your emotions, do not put good or bad, instead use the emotions in the following Plutchik's wheel of emotions:
![Plutchik's wheel of emotions](https://lh6.googleusercontent.com/6mYsdeRbzIP49QVuvc2itDoYAXCEaT-edrIXYowGvK-uuLzbXGxcUQNtfrxd96f2s7eyU9FnWkO9T6wk57GFmf_JGmathoeSurnZct7rnE3sYILL_TgDI5o4wb_2BdcmI9vUqByd)

Additionally, apart from the fact that the program runs in the terminal with Python 3, the program code will have explanation-functionality comments in the requested parts by the professor, for example, functions.

The program presents a series of questions and ends up storing it in variables to later compare each entry with what is expected for the decision-making of knowing where to channel the program; in other words, for certain questions, what you write will affect what you are asked next. At the end, it will generate an analysis of the information collected and recommendations in this regard. In the same way, it allows the user to archive everything entered through the program, generating a text file so that you can print it and attach it to your notes to discuss it with your classmates and teacher the next day of class.

Without anything else, I hope you enjoy it professor and maybe it will be useful to you.

### [](https://github.com/JuanPablo0947/pci_ad23#instrucciones)[](https://github.com/JuanPablo0947/pci_ad23#instrucciones)Interpretation of the program's statistics
Net Emotional Value (or simply, NEV) is how you measure emotion.
Calculating NEV is simple:

![equation](https://latex.codecogs.com/svg.image?nev=total\:positive\:emotions-total\:negative\:emotions&space;)

NEV grading scale:

![equation](https://latex.codecogs.com/svg.image?zero\:is\:neutral)
<br> 
![equation](https://latex.codecogs.com/svg.image?the\:greater\:from\:zero\:is\:better)
<br> 
![equation](https://latex.codecogs.com/svg.image?the\:lesser\:from\:zero\:is\:more\:bad)

Active metabolic rate (AMR) is how active you are.

AMR grading scale:
![equation](https://latex.codecogs.com/svg.image?This\:number\:ranges\:from\:1.2\:for\:being\:sedentary\\\:up\:to\:1.9\:for\:being\:very\:active.)

To understand deeply the behind the scenes of the computations please refer to the following links which were the basis of the program's development calculations:
 - NEV:
	 - [https://www.callcentrehelper.com/how-to-measure-customer-emotion-118800.htm](https://www.callcentrehelper.com/how-to-measure-customer-emotion-118800.htm)
 - AMR:
	 - [https://www.verywellfit.com/how-many-calories-do-i-need-each-day-2506873](https://www.verywellfit.com/how-many-calories-do-i-need-each-day-2506873)
	 - [https://www.mayoclinic.org/healthy-lifestyle/weight-loss/in-depth/calorie-calculator/itt-20402304](https://www.mayoclinic.org/healthy-lifestyle/weight-loss/in-depth/calorie-calculator/itt-20402304)
 - Calories:
 	 - [https://www.health.harvard.edu/staying-healthy/calorie-counting-made-easy](https://www.health.harvard.edu/staying-healthy/calorie-counting-made-easy)
 	 - [https://www.hss.edu/conditions_burning-calories-with-exercise-calculating-estimated-energy-expenditure.asp](https://www.hss.edu/conditions_burning-calories-with-exercise-calculating-estimated-energy-expenditure.asp)
 	 - https://news.sanfordhealth.org/sports-medicine/weight-gain-performance/
- Minor sources:
 	 - [Google search results one](https://www.google.com/search?q=what+is+the+percentage+of+macronutrients+a+day%3F&rlz=1C1PASC_enMX1040MX1040&oq=what+is+the+percentage+of+macronutrients+a+day%3F&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigATIHCAIQIRigATIKCAMQIRgWGB0YHjIKCAQQIRgWGB0YHtIBCDk4NTZqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8)
 	 - [Google search results two](https://www.google.com/search?q=How+many+calories+should+I+increse+to+gain+one+or+two+pounds+&newwindow=1&sca_esv=562394728&rlz=1C1PASC_enMX1040MX1040&sxsrf=AB5stBiqJZtrX6Hc4NBLzD0JyUz0LCIN8Q%3A1693780147549&ei=swj1ZMeRIdjJkPIPurqv6A0&ved=0ahUKEwiHt5bgvo-BAxXYJEQIHTrdC90Q4dUDCBA&uact=5&oq=How+many+calories+should+I+increse+to+gain+one+or+two+pounds+&gs_lp=Egxnd3Mtd2l6LXNlcnAiPUhvdyBtYW55IGNhbG9yaWVzIHNob3VsZCBJIGluY3Jlc2UgdG8gZ2FpbiBvbmUgb3IgdHdvIHBvdW5kcyBIxKUBUM0KWPmhAXAFeAGQAQCYAbUBoAGwJaoBBTM1LjE0uAEDyAEA-AEBwgIKEAAYRxjWBBiwA8ICBRAhGKABwgIFECEYqwLCAggQIRgWGB4YHcICChAhGKABGMMEGArCAgQQIRgKwgIIECEYoAEYwwTCAggQABiJBRiiBMICBRAAGKIE4gMEGAAgQYgGAZAGCA&sclient=gws-wiz-serp)
 	 - [Google search results three](https://www.google.com/search?q=Excercise+burn+calories+harvard&newwindow=1&sca_esv=562371431&sxsrf=AB5stBhdZ6dMHhTnKM4-kuVzy6_eBfo-rw%3A1693769891849&ei=o-D0ZPm5M9OQur8P_dOliAo&ved=0ahUKEwi5l_DFmI-BAxVTiO4BHf1pCaEQ4dUDCBA&uact=5&oq=Excercise+burn+calories+harvard&gs_lp=Egxnd3Mtd2l6LXNlcnAiH0V4Y2VyY2lzZSBidXJuIGNhbG9yaWVzIGhhcnZhcmQyBxAhGKABGAoyBxAhGKABGAoyCBAhGBYYHhgdSLAMUDBYtwpwAXgBkAEAmAGBAaABkgaqAQM2LjK4AQPIAQD4AQHCAgoQABhHGNYEGLADwgIHEAAYDRiABMICBhAAGB4YDcICCBAAGB4YDRgPwgIGEAAYFhgewgIIEAAYFhgeGA_CAggQABgIGB4YDcICCBAAGIoFGIYD4gMEGAAgQYgGAZAGCA&sclient=gws-wiz-serp)
 	 - https://www.healthline.com/health/what-exercise-burns-the-most-calories
 	 - [Google search results four](https://www.google.com/search?q=if+i+want+to+lose+1+to+2+lbs+by+excercise%3F&rlz=1C1PASC_enMX1040MX1040&oq=if+i+want+to+lose+1+to+2+lbs+by+excercise%3F&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIJCAEQIRgKGKABMgkIAhAhGAoYoAEyCQgDECEYChigAdIBCTEwNTgyajBqN6gCALACAA&sourceid=chrome&ie=UTF-8)
 	 - https://www.womenshealthmag.com/weight-loss/a39574131/how-to-lose-2-pounds-per-week/
 	 - [Google search results five](https://www.google.com/search?q=amr+nutritiom+stands+for&newwindow=1&sca_esv=562426022&rlz=1C1PASC_enMX1040MX1040&sxsrf=AB5stBhaa0_Nizy9vvfRMp7LJlOrYBhvhg%3A1693796748453&ei=jEn1ZLTAFf_NkPIPl5m96Aw&ved=0ahUKEwi0tofM_I-BAxX_JkQIHZdMD80Q4dUDCBA&uact=5&oq=amr+nutritiom+stands+for&gs_lp=Egxnd3Mtd2l6LXNlcnAiGGFtciBudXRyaXRpb20gc3RhbmRzIGZvcjIHECEYoAEYCjIFECEYqwIyCBAhGBYYHhgdMggQIRgWGB4YHTIIECEYFhgeGB0yCBAhGBYYHhgdMgoQIRgWGB4YDxgdSJQPUNACWOYNcAF4AZABAJgBjAGgAdYJqgEDMi45uAEDyAEA-AEBwgIKEAAYRxjWBBiwA8ICBhAAGBYYHsICCBAAGIoFGIYD4gMEGAAgQYgGAZAGCA&sclient=gws-wiz-serp)
 
### [](https://github.com/JuanPablo0947/pci_ad23#instrucciones)[](https://github.com/JuanPablo0947/pci_ad23#instrucciones)Instructions

Download the file and run the following command in the terminal:

```
python main.py
```

Conversely, you can open your IDE and hit the play button—choose whatever is comfortable to you.

Please respond to the program's prompts, the program has instructions and do not use non-standard libraries or packages.

#  [](https://github.com/JuanPablo0947/pci_ad23#pseudocodigo)Pseudocode

### Entrada
fecha => string<br>
dia => string<br>
hora => string<br>
temp => string<br>
descripción desayuno => entero<br>
descripción comida => string<br>
descripción cena => string<br>
temp => int<br>
literal sin asignar => string<br>
final description => string

Nota: todas son variables que guardan una entrada con su tipo de dato respectivo excepto la que dice "literal sin asignar" que solo es pedir el input del usuario.


### Process
 1. Crear función "largest width" con un parametro de tipo arreglo con la siguiente acción:<br>
 1.1 Identifica y almacena en una variable llamada Respuesta la palabra con más caracteres en el arreglo<br>
 1.2 Devolver el numero entero de caracteres de Respuesta
 
 2. Crear función "generate spaces" con un parametro entero con la siguiente acción:<br>
	 2.1 Asignar un string vacio a la variable "string"<br>
	 2.1 Repetir de cero hasta parametro + 1 la concatenación de un espacio a "string".
	 
 3. A la variable "printable file" asignar un objecto archivo de texto con modo de escritura/write.
 4. Pedir al usuario la fecha de hoy y asignarlo a la variable de texto "fecha".
 5. Escribir en la variable "printable file" el valor de la variable "fecha".
 6. Pedir al usuario el día de hoy y asignarlo a la variable de texto "dia".
 7. Escribir en la variable "printable file" el valor de la variable "dia".
 8. Pedir al usuario la hora de hoy y asignarlo a la variable de texto "hora".
 9. Escribir en la variable "printable file" el valor de la variable "hora".
 10. Pedir al usuario que diga si desayuno o no y asignarlo en la variable "temp"  
 11. Si el valor de la variable "temp" es igual a "Si", "si", "SI", o "sI", entonces: <br>
 11.1 Pedir al usuario que diga qué fue lo que desayuno y asignarlo a la variable "descripción desayuno"  <br>
 11.2 Escribir en la variable "printable file" el valor de la variable "descripción desayuno" con saltos de línea antes y después del valor de "descripción desayuno"
 12. Pedir al usuario que diga si comió o no y asignarlo en la variable "temp"  
 13. Si el valor de la variable "temp" es igual a "Si", "si", "SI", o "sI", entonces: <br>
 13.1 Pedir al usuario que diga qué fue lo que comió y asignarlo a la variable "descripción comi"  <br>
 13.2 Escribir en la variable "printable file" el valor de la variable "descripción comida" con saltos de línea antes y después del valor de "descripción comida"
 14. Pedir al usuario que diga si ceno o no y asignarlo en la variable "temp"  
 15. Si el valor de la variable "temp" es igual a "Si", "si", "SI", o "sI", entonces: <br>
 15.1 Pedir al usuario que diga qué fue lo que ceno y asignarlo a la variable "descripción cena" <br> 
 15.2 Escribir en la variable "printable file" el valor de la variable "descripción cena" con saltos de línea antes y después del valor de "descripción cena"
 16. Pedir al usuario que escriba la cantidad de snacks que tuvo, poniendo cero si no aplica, y asignar lo pedido a la variable "temp".
 17. Si el valor de la variable "temp" es mayor a cero, entonces:<br>
 17.1 Crear la variable "snacks" y asignar un arreglo vació al mismo.<br>
 17.2 Repetir de uno hasta "temp" + 1 el pedir lo que ceno el usuario en el snack correspondiente y agregar hasta el final de la lista "snacks" su entrada/input.<br>
 17.3 Escribir en la variable "printable file" el valor recientemente agregado a la lista de "snacks" con saltos de línea antes y después del valor de "snacks"<br>
 
 18. Crear la variable "emociones" y asignar un arreglo vació al mismo.
 19. Escribir en pantalla las indicaciones de como ingresar las emociones. 
 20. Pedir al usuario que solo escriba una emoción y después de un enter, para asignarlo a la variable "temp".
 21. Mientras el usuario no ingrese nada mas que un enter, entonces:<br>
 21.1 Agregar hasta el final de la lista "emociones" el valor de la variable "temp".<br>
 21.2 Pedir al usuario que solo escriba una emoción y después de un enter, para asignarlo a la variable "temp".
 
 22. Ciclar por cada elemento del arreglo "emociones", en cada ciclo remplazar cada elemento correspondiente por un arreglo que tiene como primer elemento la emoción/valor del elemento correspondiente a reemplazar y pedir por que el usuario siente la emoción correspondiente para que sea el último elemento del arreglo a insertar.  
 23. Agregar hasta al inicio de la lista anidada "emociones" un arreglo con los encabezados verticales "Emociones" y "Razón", en ese orden.
 24. Crear la variable "primera columna" y asignar un arreglo vació al mismo.
 25. Ciclar por cada celda (de arriba hacia abajo) de la primera columna de la matriz "emociones", en cada ciclo agregar la celda correspondiente de la primera columna en el final de la lista "primera columna".
 26. Invocar la función "largest width" y pasarle como argumento la lista "primera columna" para después guardar lo que regresa la función en una nueva variable llamada "largest width".
 27. Ciclar por las filas de la matriz "emociones" de manera descendente:<br>
 27.1 Si una celda de la primera columna tiene la longitud de la variable "largest width", entonces escribir en la variable "printable file" los valores de las celdas de fila correspondiente separados por un solo espacio con un salto de línea después de ella. <br>
 28.1 Si una celda de la primera columna tiene menor longitud de la variable "largest width", entonces escribir en la variable "printable file" los valores de las celdas de fila correspondiente separados por la cantidad de espacios generados por la función "generate spaces" que pasa como argumento la resta entre el entero de la variable "largest width" y la longitud de la celda de la primera columna correspondiente, con un salto de línea al final.
 28. Escribir en la variable "printable file" dos saltos de línea.
 29. Pedir al usuario si quiere escribir algo mas de manera libre y asignarlo en la variable "final description".
 30. Separar por intervalos de 54 caracteres el valor de texto de la variable "final description" y asignarlos consecutivamente en una lista de forma ordenada para después esta lista de pedazos de texto ser guardado en la variable "final_des".
 31. Por cada elemento de la lista "final_des" escribir su valor en la consola/terminal con un salto de linea después del mismo.
 32. Cerrar el objeto en la variable "printable file".


### Output

printable file => archivo.txt

# core-code-from-scratch-readme
core code

# DIA MARTES

## 1) El lenguaje compilado  lo traduce directamente la computadora  sin necesidad de un programa ó aplicación. Ahora el lenguaje interpretado no lo traduce directamente una computadora sino que  utiliza un programa que realiza ése proceso a travéz de el código fuente.

##2.  JAVA ES UN LENGUAJE HÍBRIDO, ya que primero se compila por un grupo de bytes para que el JRE lo pueda comprender, Luego ése grupo de bytes es interpretado por la Java Virtual Machine JVM  pasando así  a ser un lenguaje interpretado.


##3. SOLUCIÓN AL ALGORITMO DE CONVERSIÓN DE MONEDA:
`imprimir "INGRESE LA CANTIDAD EN DÓLARES"
	leer dolares
	//precio del bitcoin en dólares investigado en google.
	bitcoin = dolares * 0.000023
	
	imprimir "La conversión a bitcoin es: ",bitcoin`
   DÍA MIERCOLES
   # DÍA MIERCOLES.
  `Algoritmo sin_titulo`
	mprimir "ingrese el numero
	leer dato`
	
	dato = trunc(dato)`
	
	Si dato>0 Entonces
		Mientras dato>0 Hacer
		final = dato % 2=0
		Si final Entonces
			binario = "0" + binario
		SiNo
			binario = "1" + Binario
		Fin Si
		dato = trunc(dato/2)
		Fin Mientras
	SiNo
		Si dato=0 Entonces
			imprimir dato
		SiNo
			imprimir "el numero es negativo"
		Fin Si
	Fin Si
	
FinAlgoritmo


# DÍA JUEVES.

## Ejercicio 1:

	`let aumento=0;
	for (let i = 0; i <= 50; i++) {
 	 aumento = aumento + 2;
 	 console.log(aumento);
	}`

## Ejercicio 2:

El error fue el doble parentesis utilizado en la función IF.
únicamente se utiliza un parentesis de apertura y uno de cierre. Además
en la comparación debe tener dos ==
el codigo correcto sería:

	`var  cond  =  falso ;

	var cond = false;

	if ((cond == true)) {
	  console.log('The cond variable is true');
	} else {
	  console.log('The cond variable is false');
	}`

## Ejercicio 3:

SOLUCIÓN:
	`var n = 100;

	if (n ==100){
	    console.log('this is a special number!!');
	}

	if (n<1000 && n % 10 ==0 && n!=100) {
	    console.log('this number is almost special ');
	} else {
	    console.log('just a regular number');
	}`

# SEMANA 2 

## DÍA MARTES

**EJERCICIO 1: MULTIPLICACION**

`multiply = function (a, b) {
  return a * b;
}`

**EJERCICIO2:  ASCII**

`function uniTotal (string) {
// total up dem unicodes!
  let acumular=0;
  for(i=0;i<string.lenght; i++) {
    let ascii = string.charCodeAt(i);
    acumular = acumular + ascii;
  }
  return acumular;
}`

**EJERCICIO3: Char From   ASCII**

`function getChar(c){
  // ...
  let valor = String.fromCharCode(c);
  return valor;
}`

**EJERCICIO4: Convert dec-Binary**

`function addBinary(a,b) {
  let suma = a + b;
  const binary = suma.toString(2);
  return binary;   
}`

**EJERCICIO5: Student's final grade**

`function finalGrade (exam, projects) {
  if (exam>90 || projects>10) {
    return 100;
  } else if(exam>75 && projects>=5) {
    return 90;
  } else if (exam>50 && projects>=2){
    return 75;
  }
  return 0;
}


## DIA MIERCOLES

**Ejercicio 1**
`function dutyFree(normPrice, discount, hol){
  let AhorroUnit =  (normPrice * discount)/100;
  let res = hol/AhorroUnit;
  return Math.trunc(res);
}`

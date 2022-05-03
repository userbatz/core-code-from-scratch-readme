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
	}`


## DIA MIERCOLES

**EJERCICIO 1: Vacaciones**

	`function dutyFree(normPrice, discount, hol){
	  let AhorroUnit =  (normPrice * discount)/100;
	  let res = hol/AhorroUnit;
	  return Math.trunc(res);
	}`
	
**EJERCICIO2: Edad padre/hijo**

	`function twiceAsOld(dadYearsOld, sonYearsOld) {
	  // your code here
	  let val = dadYearsOld/2;
	  if (val<=sonYearsOld){
	    //return sonYearsOld - val;
	    return (sonYearsOld*2) -dadYearsOld;
	  }
	  return dadYearsOld- (sonYearsOld * 2);

	}`
	
**EJERCICIO 3: VALID SPACING**
	`function validSpacing(s) {

	  if(s.charAt(0) === ' ' || s.charAt(s.length - 1) === ' ') { 
	     return false;
	  }

	  for(let i = 0; i < s.length; i++) {
	    if(s.charAt(i) === ' ')
	    { 
	      if(i != 0 && s.charAt(i-1) === ' ') {
		return false;
	      }
	      if(i != (s.length - 1) && s.charAt(i+1) === ' ') {
		return false;
	      }
	    }

	  }

	  return true; 
	}`
	
**EJERCICIO 4: binario**

	`
	function fakeBin(x){
	  let nuevo = '';
	  for(i=0; i<=x.length-1;i++){
	    if(parseInt(x[i])<5){
	      nuevo = nuevo + '0';
	    } else {
	      nuevo = nuevo + '1';
	    }
	  }

	  return nuevo;
	}
	`
## DÍA JUEVES:

**Ejercicio 1: exclamation marks series**

	`function remove(string) {

	  for(i=string.length-1;i>=0;i--){   
	    if(string.substring(i,i+1)=='!') {
	      string= string.slice(0,string.length-1);
	    }
	    else {
	      break;
	    }

	  }
	  return string;
	}
	`
	
**EJERCICIO 2: vowel remover**

	`function shortcut (string) {
	  let newData = string.replace(/[aeiou]/g, '')
	  return newData;
	}`

**EJERCICIO 3: piedra papel o tijeras**

	`const rps = (p1, p2) => {
	  if(p1=='scissors' && p2=='paper' ||  p1=='paper' && p2=='rock' || p1=='rock' && p2=='scissors'){
	    return 'Player 1 won!';
	  } else if(p1=='paper' && p2=='scissors' ||  p1=='rock' && p2=='paper' || p1=='scissors' && p2=='rock') {
	    return 'Player 2 won!';
	  } else {
	    return 'Draw!';
	  }
	};`
	
**EJERCICIO 4: persistent bugger**

	`function persistence(num) {

	  let newV=[];
	  let guardar=1;
	  let cont=0;
	   while(num>=10){
	     newV = num.toString().split('');
	     for (let i = 0; i < digits.length; i++) {
	      guardar = guardar * newV[i];
	    }

	     num = guardar;
	     cont = cont +1;
	   }
	  return cont;
	}`
	
# SEMANA 3

## DÍA LUNES

**EJERCICIO 1**

	`function likes(names) {
	  // TODO
	  let texto = '';
	  if(names==''){
	    return 'no one likes this';
	  } else {
	    if(names.length==1){
	      texto = `${names} likes this`;
	    } else if(names.length==2){
	      texto = `${names[0]} and ${names[1]} like this`;
	    } else if(names.length==3){ 
	      texto = `${names[0]}, ${names[1]} and ${names[2]} like this`;
	    }  else {
	      texto = `${names[0]}, ${names[1]} and ${names.length-2} others like this`;  
	    }
	  }
	  return texto;
	}`

**EJERCICIO 2**

	`var countBits = function(n) {
	  // Program Me
	  let count=0;
	  let nuevo = n.toString(2)
	  let dato1 = nuevo.split('');

	  for(i=0;i<nuevo.length;i++){
	    if(dato1[i]=='1'){
	      count += 1;
	    }
	  }`
	 
**EJERCICIO 3**

	`function order(words) {
	  // ...
	  let texto = words.split(' ');
	  let cont = 0;
	  let id = [];
	  let txt = [];
	  let aux = 0;
	  let aux1 = 0;

	  if(words == ''){
	    return '';
	  }
	  for (i = 0; i < texto.length; i++) {

	    let contenido = texto[i].split('');

	    for (j = 0; j < contenido.length; j++) {
	      if (isNaN(contenido[j]) == false) {
		id[cont] = parseInt(contenido[j], 10);
		txt[cont] = texto[i];
		cont += 1;
	      }
	    }

	  }
	  for (k = 1; k < id.length; k++) {
	    for (i = 0; i < (id.length - k); i++) {
	      if (id[i] > id[i + 1]) {
		aux = id[i];
		aux1 = txt[i];
		id[i] = id[i + 1];
		txt[i] = txt[i + 1];
		id[i + 1] = aux;
		txt[i + 1] = aux1;
	      }
	    }
	  }

	  return txt.join(' ');

	}`
	
## DÍA MARTES

**EJERCICIO 1**

	`function pigIt(str){
	  //Code here
	  let texto = str.split(' ');
	  let indv = '';
	  console.log(texto);
	  for(i=0;i<texto.length;i++){
	    indv = texto[i].split('');
	    indv.push(indv[0]);
	    indv.shift();
	    indv.push('ay');
	    indv.join('');
	    texto[i]=indv;
	    console.log(texto[i].join('')); 



	}
	return texto.join('  ');
	}`
	
**EJERCICIO 2**

	`function duplicateCount(text){
	  //...
	  let contador=0;
	  let count = [];
	  let newText = text.toLowerCase();
	  let txt = newText.split('');
	  txt.sort();

	  if(txt[0]!=txt[1]){
	    return 0;
	  }

	  while (txt[0]==txt[contador+1]){
	    contador +=1;
	  }

	  return contador+1;
	}`
	
**EJERCICIO 3**

	`function (morseCode) {
	  morseCode = morseCode.replace(/   /g, '#');
	  let decodedCode = '';
	  let tempWordToDecode = '';
	  for (let i = 0, lenght = morseCode.length; i < lenght; i++) {
	    if (morseCode[i] === ' ') {
	      decodedCode += MORSE_CODE[tempWordToDecode] || '';
	      tempWordToDecode = '';
	    } else if (morseCode[i] === '#') {
	      decodedCode += `${MORSE_CODE[tempWordToDecode] || ''} `;
	      tempWordToDecode = '';
	    } else {
	      tempWordToDecode += morseCode[i];
	    }
	  }
	  decodedCode += MORSE_CODE[tempWordToDecode] || '';
	  return decodedCode.trim();
	};`

## DIA MIERCOLES

**EJERCICIO 1**

	`function validParentheses(parens) {
	  // your code here ..
	  let nw = parens.split('');
	  let cont = 0;
	  let total = 0;
	  for(i=0;i<nw.length;i++){
	    if(nw[i]=='('){
	      cont = 1;
	    } else {
	      cont = -1;
	    }


	    total += cont;
	  }

	  if(total==0){
	    return true;
	  }
	  return false;

	}`
	
**EJERCICIO 2**

	`function toCamelCase(str) {
	  let res = '';
	  for (let i = 0; i < str.length; i++) {
	    if (i != 0 && (str[i - 1] === '_' || str[i - 1] === '-')) {
	      res += str[i].toUpperCase();
	    } else if (str[i] != '-' && str[i] != '_') {
	      res += str[i];
	    }
	  }
	  return res;
	}`

**EJERCICIO 3**

	`function uniqueInOrder(iterable) {

	  let nwT; 
	  let res = [];
	  let range= iterable.length;


	  for (let i = 0; i < range; i++) {

	    if (iterable[i] !== nwT) {
	      nwT = iterable[i];
	      res.push(nwT);
	    }


	  }

	  return res;
	}`
	
	
## DIA JUEVES

**EJERCICIO 1**

	`function foldArray(array, runs)
	{
	    let leftEnd = Math.floor(array.length / 2),
		rightStart = Math.ceil(array.length / 2);

	    let left = array.slice(0, leftEnd),
		right = array.slice(rightStart).reverse();

	    let result = left.map((val, index) => {
		return val + right[index];
	    });

	    if (leftEnd !== rightStart) {
		result.push(array[leftEnd]);
	    }

	    return runs === 1 ? result : foldArray(result, runs - 1);
	}`


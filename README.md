Algoritmo Menu_Ejercicios_Logica
	Definir opcion Como Entero
	Repetir
		Escribir "=============== MENU ==============="
		Escribir "1. Números"
		Escribir "2. Cadenas y Arreglos"
		Escribir "3. Salir"
		Escribir "====================================="
		Escribir "Ingrese una opción: "
		Leer opcion
		Segun opcion Hacer
			1: 
				Repetir
					Escribir "=============== MENU ==============="
					Escribir "1. Determinar el costo de la venta de gaseosas"
					Escribir "2. Determinar la ganancia obtenida de la asociación de vinicultores"
					Escribir "3. Dado dos números obtener el residuo sin el operador mod, % "
					Escribir "4. Determinar el valor de la cita del consultorio del Dr. Paez"
					Escribir "5. Escribir un algoritmo que lea cuatro números y determine si el numero 1  es la mitad del número 2; Y si el numero 3 es divisor del numero4. "
					Escribir "6. Determinar el limite de credito para el banco XYZ"
					Escribir "7. Escribir un algoritmo que lea cuatro números y determine si el numero 1 es divisor del numero3 Y si el numero 2 es el doble del numero4. "
					Escribir "8. Determinar el límite de credito para el banco POO"
					Escribir "9. Pedir al usuario un número y mostrar si es negativo menor que -20, sino mostrar si es positivo par o impar múltiplo de 7."
					Escribir "10. Determinar el precio de embarque para la asociacón de vinicultores"
					Escribir "11. Pedir al usuario un número y mostrar si es par menor que 10, sino mostrar si es negativo e impar o negativo divisible para 5. "
					Escribir "12. Determinar los precios de venta de fábricas El cometa"
					Escribir "13. Dado un número entero N, calcular e informar al usuario cuántos dígitos tiene dicho número. "
					Escribir "14. Dado un número, determine si es capicúa."
					Escribir "15. Escribir un algoritmo que presente los divisores de un numero "
					Escribir "16. Escribir un algoritmo que presente la suma de los divisores de un numero "
					Escribir "17. Escribir un algoritmo que presente la cantidad de los divisores de un numero "
					Escribir "18. Escribir un algoritmo que indique si un número es perfecto "
					Escribir "19. Dado un número N determinar si es un número primo. "
					Escribir "20. Dado dos números determinar si son  primos gemelos. "
					Escribir "21. Dado dos números determinar si son  primos amigos. "
					Escribir "====================================="
					Escribir "Ingrese una opción: "
					Leer opcion
					Segun opcion Hacer
					1:
								Definir cantidadColas, costoBase, costoTotalSinIVA, iva, totalAPagar Como Real
								
								Escribir "Ingrese la cantidad de colas compradas:"
								Leer cantidadColas
								
								Si cantidadColas > 23 Entonces
									costoBase = 0.50
								Sino
									costoBase = 1.20
								FinSi
								
								costoTotalSinIVA = cantidadColas * costoBase
								iva = 0.12 * costoTotalSinIVA
								totalAPagar = costoTotalSinIVA + iva
								
								Escribir "Cantidad comprada:", cantidadColas
								Escribir "Costo por unidad: $", costoBase
								Escribir "Total sin IVA: $", costoTotalSinIVA
								Escribir "IVA (12%): $", iva
								Escribir "Total a pagar: $", totalAPagar
						2:
							Definir kilos, precioInicial Como Real
							Definir tipo Como Caracter
							Definir tamano Como Entero
							Definir ganancia Como Real
							
							Escribir "El siguiente algoritmo se encarga de calcular la ganancia de acuerdo a el tipo de uva, tamaño y la cantidad vendida."
							Escribir "Ingrese el número de kilos entregados por el productor:"
							Leer kilos
							Escribir "Ingrese el precio inicial por kilo:"
							Leer precioInicial
							Escribir "Ingrese el tipo de uva (A o B):"
							Leer tipo
							Escribir "Ingrese el tamaño de la uva (1 o 2):"
							Leer tamano
							
							Si (tipo = "A") Entonces
								Si (tamano = 1) Entonces
									ganancia = (precioInicial * kilos) + (kilos * 0.20)
								Sino
									ganancia = (precioInicial * kilos) + (kilos * 0.30)
								FinSi
							Sino
								Si (tamano = 1) Entonces
									ganancia = (precioInicial * kilos) - (kilos * 0.30)
								Sino
									ganancia = (precioInicial * kilos) - (kilos * 0.50)
								FinSi
							FinSi
							
							Escribir "La ganancia obtenida es: ", ganancia
						3: 
							Definir num1, num2, cociente, residuo Como Entero
							Escribir "Ingrese el primer número (dividendo):"
							Leer num1
							Escribir "Ingrese el segundo número (divisor):"
							Leer num2
							Si num2 = 0 Entonces
								Escribir "El divisor no puede ser cero."
							Sino
								cociente <- Trunc(num1 / num2)
								residuo <- num1 - (num2 * cociente)
								Escribir "El residuo de la división es: ", residuo
							FinSi
						4:
							Definir num_cita, costo_cita, total_pagado Como Real
							Escribir "Ingrese el número de cita:"
							Leer num_cita
							total_pagado = 0
							Si num_cita <= 3 Entonces
								costo_cita = 200
								total_pagado = num_cita * 200
							Sino
								Si num_cita <= 5 Entonces
									costo_cita = 150
									total_pagado = 3 * 200 + (num_cita - 3) * 150
								Sino
									Si num_cita <= 8 Entonces
										costo_cita = 100
										total_pagado = 3 * 200 + 2 * 150 + (num_cita - 5) * 100
									Sino
										costo_cita = 50
										total_pagado = 3 * 200 + 2 * 150 + 3 * 100 + (num_cita - 8) * 50
									FinSi
								FinSi
							FinSi
							Escribir "El costo de la cita es: $", costo_cita
							Escribir "El total pagado hasta la cita ", num_cita, " es: $", total_pagado	
						5:
							Definir num1, num2, num3, num4 Como Real
							Escribir "Ingrese el primer número:"
							Leer num1
							Escribir "Ingrese el segundo número:"
							Leer num2
							Escribir "Ingrese el tercer número:"
							Leer num3
							Escribir "Ingrese el cuarto número:"
							Leer num4
							Si num1 = num2 / 2 Entonces
								Escribir "El primer número es la mitad del segundo número."
							SiNo
								Escribir "El primer número no es la mitad del segundo número."
							FinSi
							Si num4 % num3 = 0 Entonces
								Escribir "El tercer número es divisor del cuarto número."
							SiNo
								Escribir "El tercer número no es divisor del cuarto número."
							FinSi
						6:
							Definir tipoTarjeta Como Entero
							Definir limiteActual, nuevoLimite Como Real
							Escribir "Ingrese el tipo de tarjeta (1, 2, 3, otro):"
							Leer tipoTarjeta
							Escribir "Ingrese el límite de crédito actual:"
							Leer limiteActual
							Segun tipoTarjeta Hacer
								1:
									nuevoLimite = limiteActual * 1.25
								2:
									nuevoLimite = limiteActual * 1.35
								3:
									nuevoLimite = limiteActual * 1.40
								De Otro Modo:
									nuevoLimite = limiteActual * 1.50
							FinSegun
							nuevoLimite = nuevoLimite + 20
							Escribir "El nuevo límite de crédito es: ", nuevoLimite
						7:
							Definir num1, num2, num3, num4 Como Real
							Escribir "Ingrese el primer número:"
							Leer num1
							Escribir "Ingrese el segundo número:"
							Leer num2
							Escribir "Ingrese el tercer número:"
							Leer num3
							Escribir "Ingrese el cuarto número:"
							Leer num4
							Si num1 = num2 / 2 Entonces
								Escribir "El primer número es la mitad del segundo número."
							SiNo
								Escribir "El primer número no es la mitad del segundo número."
							FinSi
							Si num4 % num3 = 0 Entonces
								Escribir "El tercer número es divisor del cuarto número."
							SiNo
								Escribir "El tercer número no es divisor del cuarto número."
							FinSi
						8:
								Definir tipoTarjeta Como Entero
								Definir limiteActual Como Real
								Definir aumentoInicial Como Real
								Definir nuevoLimite Como Real
								Escribir "Ingrese el tipo de tarjeta (1, 2, 3 o cualquier otro número): "
								Leer tipoTarjeta
								Escribir "Ingrese el límite de crédito actual: "
								Leer limiteActual
								Segun tipoTarjeta Hacer
									1:
										aumentoInicial = 100
									2:
										aumentoInicial = 200
									3:
										aumentoInicial = 300
									De Otro Modo:
										aumentoInicial = 500
								FinSegun
								nuevoLimite = limiteActual + aumentoInicial
								nuevoLimite = nuevoLimite * 1.10
								Escribir "El nuevo límite de crédito es: ", nuevoLimite
						9:
								Definir numero Como Real
								Escribir "Ingrese un número:"
								Leer numero
								Si numero < -20 Entonces
									Escribir "El número es negativo y menor que -20."
								Sino
									Si numero > 0 Entonces
										Si numero % 2 = 0 Entonces
											Escribir "El número es positivo y par."
										Sino
											Si numero % 7 = 0 Entonces
												Escribir "El número es positivo, impar y múltiplo de 7."
											Sino
												Escribir "El número es positivo e impar."
											FinSi
										FinSi
									Sino
										Escribir "El número no cumple con las condiciones especificadas."
									FinSi
								FinSi
						10:
								Definir tipo Como Cadena
								Definir tamano Como Entero
								Definir precio_inicial, precio_final, precio_con_iva, descuento, iva Como Real
								Escribir "Ingrese el tipo de pitahaya (Amarilla/Colorada): "
								Leer tipo
								Escribir "Ingrese el tamaño de la pitahaya (1/2): "
								Leer tamano
								Escribir "Ingrese el precio inicial del quintal: "
								Leer precio_inicial
								
								precio_final = precio_inicial
								Si tipo = "Amarilla" Entonces
									Si tamano = 1 Entonces
										precio_final = precio_inicial + 10
									SiNo
										precio_final = precio_inicial * 1.15 + 5
									FinSi
								finsi
								Si tipo = "Colorada" Entonces
									Si tamano = 1 Entonces
										precio_final = precio_inicial - 20
									SiNo
										precio_final = precio_inicial * 0.80
									FinSi
								finsi
								descuento = precio_final * 0.05
								precio_final = precio_final - descuento
								
								iva = precio_final * 0.12
								precio_con_iva = precio_final + iva
								Escribir "El precio de embarque es: $", precio_con_iva
						11:
								Definir numero Como Entero
								Escribir "Introduce un número:"
								Leer numero
								Si numero MOD 2 = 0 Entonces
									
									Si numero < 10 Entonces
										Escribir "El número es par y menor que 10."
									SiNo
										Escribir "El número es par y mayor o igual a 10."
									FinSi
								SiNo
									
									Si numero < 0 Entonces
										// Si es negativo
										Si numero MOD 5 = 0 Entonces
											Escribir "El número es negativo e impar y divisible por 5."
										SiNo
											Escribir "El número es negativo e impar."
										FinSi
									SiNo
										Escribir "El número es positivo e impar."
									FinSi
								FinSi
						12:
								Definir clave, materiaPrima, manoDeObra, gastosFabricacion, costoProduccion, precioVenta como Real
								
								Escribir "Ingrese la clave del producto (1, 2, 3, 4, 5 o 6):"
								Leer clave
								
								Escribir "Ingrese el costo de la materia prima:"
								Leer materiaPrima
								
								Si clave = 3 o clave = 4 Entonces
									manoDeObra = 0.75 * materiaPrima
									Si clave = 1 o clave = 5 Entonces
										manoDeObra = 0.80 * materiaPrima
									Sino
										manoDeObra = 0.85 * materiaPrima
									FinSi
								FinSi
								
								
								Si clave = 2 o clave = 5 Entonces
									gastosFabricacion = 0.30 * materiaPrima
									Si clave = 3 o clave = 6 Entonces
										gastosFabricacion = 0.35 * materiaPrima
									Sino
										gastosFabricacion = 0.28 * materiaPrima
									finsi
								FinSi
								
								costoProduccion = materiaPrima + manoDeObra + gastosFabricacion
								precioVenta = costoProduccion + 0.45 * costoProduccion
								
								Escribir "El precio de venta del producto es:", precioVenta	
						13:
								Definir numero, contador Como Entero
								
								Escribir "Ingrese un número entero:"
								Leer numero
								
								contador <- 0
								
								Mientras numero <> 0 Hacer
									numero <- numero / 10
									contador <- contador + 1
								Fin Mientras
								
								Escribir "El número tiene ", contador, " dígitos."
								
						14:
								Escribir "Ingrese un número:"
								Leer numero
								
								
								numeroOriginal = numero
								numeroInvertido = 0
								Mientras numero > 0
									resto = numero % 10
									numeroInvertido = numeroInvertido * 10 + resto
									numero = numero / 10
								Fin Mientras
								
								Si numeroOriginal = numeroInvertido Entonces
									Escribir "El número ingresado es capicúa."
								Sino
									Escribir "El número ingresado no es capicúa."
								Fin Si
						15:
								Definir numero, divisor Como Entero
								Escribir "Ingrese un número:"
								Leer numero
								
								Escribir "Los divisores de", numero, "son:"
								Para divisor = 1 Hasta numero
									Si numero % divisor = 0 Entonces
										Escribir divisor
									Fin Si
								Fin Para
						16:	
								Escribir "Ingrese un número:"
								Leer numero
								sumaDivisores <- 0
								
								Para i <- 1 Hasta numero Con Paso 1 Hacer
									
									Si numero MOD i == 0 Entonces
										sumaDivisores <- sumaDivisores + i
									FinSi
								FinPara
								Escribir "La suma de los divisores de ", numero, " es: ", sumaDivisores
						17:
								Definir numero, suma, divisor como Entero
								
								Escribir "Ingrese un número:"
								Leer numero
								suma <- 0
								Para divisor <- 1 Hasta numero Hacer
									Si numero MOD divisor == 0 Entonces
										suma <- suma + divisor
									FinSi
								FinPara
								
								Escribir "La suma de los divisores de ", numero, " es: ", suma
						18:
								Definir numero, sumaDivisores, divisor Como Entero
								
								Escribir "Ingrese un número:"
								Leer numero
								
								sumaDivisores <- 0
								
								Para divisor <- 1 Hasta numero/2 Hacer
									Si numero MOD divisor = 0 Entonces
										sumaDivisores <- sumaDivisores + divisor
									FinSi
								FinPara
								
								Si sumaDivisores = numero Entonces
									Escribir "El número ", numero, " es perfecto."
								Sino
									Escribir "El número ", numero, " no es perfecto."
								FinSi
						19:
								Definir n, i, contador como Entero
								contador <- 0
								
								Escribir "Ingrese un número:"
								Leer n
								
								Para i <- 1 Hasta n 
									Si n % i == 0 Entonces
										contador <- contador + 1
									FinSi
								FinPara
								
								Si contador == 2 Entonces
									Escribir "El número", n, "es primo."
								Sino
									Escribir "El número", n, "no es primo."
								FinSi
						20:
								Definir num1, num2, i, cont1, cont2 como Entero
								
								Escribir "Ingrese el primer número:"
								Leer num1
								
								Escribir "Ingrese el segundo número:"
								Leer num2
								
								cont1 <- 0
								cont2 <- 0
								
								Para i <- 2 Hasta num1/2 Con Paso 1 Hacer
									Si num1 MOD i = 0 Entonces
										cont1 <- cont1 + 1
									FinSi
								FinPara
								
								Para i <- 2 Hasta num2/2 Con Paso 1 Hacer
									Si num2 MOD i = 0 Entonces
										cont2 <- cont2 + 1
									FinSi
								FinPara
								
								Si cont1 = 0 Y cont2 = 0 Y Abs(num1 - num2) = 2 Entonces
									Escribir "Los números", num1, "y", num2, "son primos gemelos."
								Sino
									Escribir "Los números ingresados no son primos gemelos."
								FinSi
						21:
								Definir num1, num2, i, j, esPrimo1, esPrimo2 como Entero
								
								Escribir "Ingrese el primer número:"
								Leer num1
								Escribir "Ingrese el segundo número:"
								Leer num2
								
								esPrimo1 = 1
								i = 2
								Mientras i < num1 Y esPrimo1
									Si num1 MOD i = 0 Entonces
										esPrimo1 = 0
									FinSi
									i = i + 1
								FinMientras
								
								esPrimo2 = 1
								j = 2
								Mientras j < num2 Y esPrimo2
									Si num2 MOD j = 0 Entonces
										esPrimo2 = 0
									FinSi
									j = j + 1
								FinMientras
								
								Si esPrimo1 Y esPrimo2 Y Abs(num1 - num2) = 2 Entonces
									Escribir "Los números", num1, "y", num2, "son primos gemelos."
								Sino
									Escribir "Los números", num1, "y", num2, "no son primos gemelos."
								FinSi
					FinSegun
				Hasta Que opcion = 21
			2:
				Repetir
					Escribir "=============== MENU ==============="
					Escribir "1. Dada n realizar un algoritmo que presente la siguiente secuencia: n=6; respuesta= 2, 2, 4, 8, 32, 256 "
					Escribir "2. Implementa un programa que calcule el promedio de los elementos pares e impares en un arreglo de números enteros y los copie en otro arreglo. "
					Escribir "3. Dada n realizar un algoritmo que presente la siguiente secuencia: n=6; respuesta= 20, 5, 15, 10, 5, -5, 0"
					Escribir "4. Implementa un programa que copie los números de un arreglo a  2 arreglos en uno  los números positivos y en el otro los negativos"
					Escribir "5. Leer una secuencia de números hasta que se ingrese un numero negativo. Mostrar la suma de los pares y la cantidad de los números que son múltiplo de 3 "
					Escribir "6. Leer una secuencia de números hasta que se ingrese un 0 y almacenarlos en un arreglo Se pide recorrer el arreglo y mostrar la suma del cuadrado de cada numero."
					Escribir "7. Leer una secuencia de números hasta que se ingrese un numero par. Mostrar la cantidad de los números mayores a 5 y la suma de los múltiplos de 5"
					Escribir "8. Dado una frase indicar cuantas palabras tiene"
					Escribir "9. Leer una secuencia de números hasta que se ingrese un numero negativo y almacenarlos en arreglo. Se pide recorrer el arreglo y cambiar cada elemento del arreglo por su doble. "
					Escribir "10. Leer una secuencia de caracteres hasta que se ingrese un punto. Deberá mostrar cuantos "x" se ingresaron  "
					Escribir "11. Leer una secuencia de números hasta que se ingrese un 0 y almacenarlos en arreglo. Se pide recorrer el arreglo y pasar a otro arreglo solo los números pares de cada elemento del arreglo1 "
					Escribir "12. Dado dos números presentar los valores mayores a 5 entre ellos incluidos el numero inicial y final "
					Escribir "13. Elaborar un algoritmo que lea una serie de edades de los alumnos de la facultad FACI y los guarde en un arreglo. "
					Escribir "14. Dado dos números presentar los valores Impares comprendidos entre ellos(excluidos el valor inicial y final "
					Escribir "15.  Elaborar un algoritmo que lea una serie de sueldos de los empleados de la unemi y los guarde en un arreglo."
					Escribir "16. Dadas dos frases indicar la de mayor longitud"
					Escribir "17. Indicar cuantas ,.;: hay en una cadena"
					Escribir "18. Dado una cadena indicar cuantas vocales, consonantes y dígitos hay" 
					Escribir "19. Indicar cuantas palabras hay en una frase asumiendo 1 o varios espacios entre palabras" 
					Escribir "20. Presentar la suma de los dígitos de una cedula"
					Escribir "21. ndicar si una palabra es palíndroma"
					Escribir "====================================="
					Escribir "Ingrese una opción: "
					Leer opcion
					Segun opcion Hacer
						1: 
								Escribir "Ingrese un número:"
								Leer numero
								sumaDivisores <- 0
								Para i <- 1 Hasta numero Con Paso 1 Hacer
									Si numero MOD i == 0 Entonces
										sumaDivisores <- sumaDivisores + i
									FinSi
								FinPara
								Escribir "La suma de los divisores de ", numero, " es: ", sumaDivisores
						2:
								Definir numeros, resultado Como Entero
								Definir i, sumaPares, sumaImpares, contPares, contImpares Como Entero
								
								Escribir "Ingrese la cantidad de elementos del arreglo: "
								Leer n
								
								Dimension numeros[n]
								Dimension resultadoPares[n]
								Dimension resultadoImpares[n]
								
								sumaPares <- 0
								sumaImpares <- 0
								contPares <- 0
								contImpares <- 0
								Para i <- 0 Hasta n - 1 Hacer
									Escribir "Ingrese el elemento ", i + 1, ": "
									Leer numeros[n]
									
									Si numeros[n] % 2 = 0 Entonces
										sumaPares <- sumaPares + numeros[n]
										resultadoPares[contPares] <- numeros[i]
										contPares <- contPares + 1
									Sino
										sumaImpares <- sumaImpares + numeros[n]
										resultadoImpares[contImpares] <- numeros[i]
										contImpares <- contImpares + 1
									FinSi
								FinPara
								Si contPares > 0 Entonces
									promedioPares <- sumaPares / contPares
								Sino
									promedioPares <- 0
								FinSi
								
								Si contImpares > 0 Entonces
									promedioImpares <- sumaImpares / contImpares
								Sino
									promedioImpares <- 0
								FinSi
								
								Escribir "El promedio de los elementos pares es: ", promedioPares
								Escribir "Los elementos pares son: "
								Para i <- 0 Hasta contPares - 1 Hacer
									Escribir resultadoPares[i], " "
								FinPara
								
								Escribir ""
								Escribir "El promedio de los elementos impares es: ", promedioImpares
								Escribir "Los elementos impares son: "
								Para i <- 0 Hasta contImpares - 1 Hacer
									Escribir resultadoImpares[i], " "
								FinPara
						3:
								Definir n, i, respuesta Como Entero
								respuesta <- 20
								Escribir respuesta
								Para i<-1 Hasta 6 Con Paso 1 Hacer
									Si i Mod 2 = 0 Entonces
										respuesta <- respuesta - 10
									Sino
										respuesta <- respuesta / 2
									FinSi
									Escribir respuesta
								FinPara
						4:
								Definir numeros, positivos, negativos Como Entero
								Definir i, contPositivos, contNegativos Como Entero
								
								Dimension numeros[5]
								numeros[0] <- 2
								numeros[1] <- -6
								numeros[2] <- 4
								numeros[3] <- -9
								numeros[4] <- 12
								
								contPositivos <- 0
								contNegativos <- 0
								Para i <- 0 Hasta 4 Hacer
									Si numeros[i] > 0 Entonces
										contPositivos <- contPositivos + 1
									Sino
										contNegativos <- contNegativos + 1
									FinSi
								FinPara
								Dimension positivos[contPositivos]
								Dimension negativos[contNegativos]
								
								contPositivos <- 0
								contNegativos <- 0
								Para i <- 0 Hasta 4 Hacer
									Si numeros[i] > 0 Entonces
										positivos[contPositivos] <- numeros[i]
										contPositivos <- contPositivos + 1
									Sino
										negativos[contNegativos] <- numeros[i]
										contNegativos <- contNegativos + 1
									FinSi
								FinPara
								Escribir "El arreglo original es: [2, -6, 4, -9, 12]"
								Escribir "Los números positivos son: "
								Para i <- 0 Hasta contPositivos - 1 Hacer
									Escribir positivos[i], " "
								FinPara
								
								Escribir ""
								Escribir "Los números negativos son: "
								Para i <- 0 Hasta contNegativos - 1 Hacer
									Escribir negativos[i], " "
								FinPara
						5:
								Definir numero, paresSuma, contMultiplos3 Como Entero
								paresSuma <- 0
								contMultiplos3 <- 0
								numero <- 0
								Mientras numero >= 0 Hacer
									Escribir "Ingrese un número (ingrese un número negativo para terminar): "
									Leer numero
									Si numero >= 0 Entonces
										Si numero Mod 2 = 0 Entonces
											paresSuma <- paresSuma + numero
										FinSi
										Si numero Mod 3 = 0 Entonces
											contMultiplos3 <- contMultiplos3 + 1
										FinSi
									FinSi
								FinMientras
								Escribir "La suma de los números pares es: ", paresSuma
								Escribir "La cantidad de números que son múltiplo de 3 es: ", contMultiplos3
						6:
								Definir numeros, exponentes Como Entero
								Definir i, j, suma Como Entero
								i <- 0
								suma <- 0
								Dimension numeros[100] 
								Repetir
									Escribir "Ingrese un número (0 para terminar): "
									Leer numeros[i]
									Si numeros[i] <> 0 Entonces
										i <- i + 1
									FinSi
								Hasta Que numeros[i] = 0
								Dimension exponentes[i]
								
								Para j <- 0 Hasta i - 1 Hacer
									exponentes[j] <- numeros[j] ^ 2
									suma <- suma + exponentes[j]
								FinPara
								Escribir "La secuencia ingresada es: "
								Para j <- 0 Hasta i - 1 Hacer
									Escribir Sin Saltar numeros[j], ", "
								FinPara
								Escribir ""
								Escribir "El arreglo de exponentes es: "
								Para j <- 0 Hasta i - 1 Hacer
									Escribir Sin Saltar exponentes[j], ", "
								FinPara
								Escribir ""
								Escribir "La suma de los cuadrados es: ", suma
						7:
								Definir numero, contMay5, sumaMultiplos5 Como Entero
								contMay5 <- 0
								sumaMultiplos5 <- 0
								numero <- 0
								Mientras numero Mod 2 <> 0 Hacer
									Escribir "Ingrese un número (ingrese un número par para terminar): "
									Leer numero
									Si numero > 5 Entonces
										contMay5 <- contMay5 + 1
									FinSi
									Si numero Mod 5 = 0 Entonces
										sumaMultiplos5 <- sumaMultiplos5 + numero
									FinSi
								FinMientras
								Escribir "La cantidad de números mayores a 5 es: ", contMay5
								Escribir "La suma de los múltiplos de 5 es: ", sumaMultiplos5
						8:
								Definir frase Como Caracter
								Definir cantidadPalabras Como Entero
								Definir i Como Entero
								Escribir "Ingrese una frase: "
								Leer frase
								cantidadPalabras <- 1
								Para i <- 0 Hasta Longitud(frase) - 1 Hacer
									Si Subcadena(frase, i, i) = " " Entonces
										cantidadPalabras <- cantidadPalabras + 1
									FinSi
								FinPara
								Escribir "La frase ingresada tiene ", cantidadPalabras, " palabras."
						9:
							Definir numero, i como Entero
							Definir secuencia_numeros como Entero
							Definir longitud_secuencia como Entero
							
							i = 1
							longitud_secuencia = 100
							Dimension secuencia_numeros[longitud_secuencia]
							
							Escribir "Ingrese una secuencia de números. Ingrese un número negativo para terminar."
							
							Repetir
								Leer numero
								Si numero >= 0 Entonces
									secuencia_numeros[i] = numero
									i = i + 1
								FinSi
							Hasta Que numero < 0
							
							Escribir "Se han almacenado los siguientes números en la secuencia:"
							
							Para j = 1 Hasta i - 1
								Escribir secuencia_numeros[j]
							FinPara
						10:
								Definir caracter Como Caracter
								Definir contadorX Como Entero
								contadorX <- 0
								Escribir "Ingrese una secuencia de caracteres (ingrese un punto para terminar): "
								Leer caracter
								Mientras caracter <> "." Hacer
									Si caracter = "x" Entonces
										contadorX <- contadorX + 1
									FinSi
									Leer caracter
								FinMientras
								Escribir "La letra x se ingresó ", contadorX, " veces."
						11:
								Definir i, j, numero, cantidadPares Como Entero
								cantidadPares <- 0
								i <- 1
								numero <- 1
								Escribir "Ingrese una secuencia de números (ingrese 0 para terminar): "
								Mientras numero <> 0 Hacer
									Leer numero
									Si numero MOD 2 = 0 Entonces
										cantidadPares <- cantidadPares + 1
									FinSi
									i <- i + 1
								FinMientras
								
								Escribir "La cantidad de números pares es: ", cantidadPares
						12:
								Definir numInicial, numFinal, i Como Entero
								Escribir "Ingrese el número inicial: "
								Leer numInicial
								Escribir "Ingrese el número final: "
								Leer numFinal
								
								Escribir "Los valores mayores a 5 entre ", numInicial, " y ", numFinal, " son: "
								Para i <- numInicial Hasta numFinal Hacer
									Si i > 5 Entonces
										Escribir i
									FinSi
								FinPara
						13:
								Definir edades[100] Como Entero
								Definir cantidadEstudiantes, sumaEdades, contadorMayores, contadorMenores Como Entero
								Definir promedioGeneral, promedioMayorIgual18, promedioMenor18 Como Real
								cantidadEstudiantes = 0
								sumaEdades = 0
								contadorMayores = 0
								contadorMenores = 0
								
								Escribir "Ingrese la cantidad de estudiantes:"
								Leer cantidadEstudiantes
								
								Para i = 1 Hasta cantidadEstudiantes Hacer
									Escribir "Ingrese la edad del estudiante ", i
									Leer edades[i]
									sumaEdades = sumaEdades + edades[i]
									Si edades[i] >= 18 Entonces
										contadorMayores = contadorMayores + 1
									Sino
										contadorMenores = contadorMenores + 1
									FinSi
								FinPara
								
								promedioGeneral = sumaEdades / cantidadEstudiantes
								Si contadorMayores > 0 Entonces
									promedioMayorIgual18 = sumaEdades / contadorMayores
								FinSi
								Si contadorMenores > 0 Entonces
									promedioMenor18 = sumaEdades / contadorMenores
								FinSi
								
								Escribir "Promedio general de edades: ", promedioGeneral
								Escribir "Cantidad de estudiantes mayores o iguales a 18: ", contadorMayores
								Escribir "Promedio de edades mayores o iguales a 18: ", promedioMayorIgual18
								Escribir "Cantidad de estudiantes menores a 18: ", contadorMenores
								Escribir "Promedio de edades menores a 18: ", promedioMenor18
						14:
								Definir valorInicial, valorFinal, i Como Entero
								
								Escribir "Ingresa el valor inicial:"
								Leer valorInicial
								Escribir "Ingresa el valor final:"
								Leer valorFinal
								
								Para i <- valorInicial + 1 Hasta valorFinal - 1 Con Paso 1 Hacer
									Si i MOD 2 <> 0 Entonces
										Escribir i
									FinSi
								FinPara
						15:
								Definir sueldos Como Numerica
								Definir sueldoMasAlto, cantidadSueldos, promedioGeneral Como Real
								Definir i Como Entero
								
								Escribir "Ingrese la cantidad de empleados: "
								Leer cantidadEmpleados
								
								Dimension sueldos(cantidadEmpleados)
								
								Para i <- 1 Hasta cantidadEmpleados Hacer
									Escribir "Ingrese el sueldo del empleado ", i, ": "
									Leer sueldos(i)
								FinPara
								
								sueldoMasAlto <- sueldos(1)
								cantidadSueldos <- cantidadEmpleados
								promedioGeneral <- 0
								
								Para i <- 1 Hasta cantidadEmpleados Hacer
									Si sueldos(i) > sueldoMasAlto Entonces
										sueldoMasAlto <- sueldos(i)
									FinSi
									promedioGeneral <- promedioGeneral + sueldos(i)
								FinPara
								
								promedioGeneral <- promedioGeneral / cantidadEmpleados
								
								Escribir "Sueldo más alto: ", sueldoMasAlto
								Escribir "Cantidad de sueldos: ", cantidadSueldos
								Escribir "Promedio general: ", promedioGeneral
						16:	
								Definir frase1, frase2 Como Cadena
								
								Escribir "Ingrese la primera frase: "
								Leer frase1
								
								Escribir "Ingrese la segunda frase: "
								Leer frase2
								
								Si Longitud(frase1) > Longitud(frase2) Entonces
									Escribir "La primera frase es más larga."
									Escribir "La segunda frase es más larga."
								Sino
									Escribir "Ambas frases tienen la misma longitud."
								FinSi
						17:
								Definir cadena Como Cadena
								Definir comas, puntos, puntoYComa, dosPuntos Como Entero
								
								Escribir "Ingrese una cadena de texto: "
								Leer cadena
								
								comas <- 0
								puntos <- 0
								puntoYComa <- 0
								dosPuntos <- 0
								
								Para i <- 0 Hasta Longitud(cadena) - 1 Hacer
									Segun Subcadena(cadena, i, i) Hacer
										Caso ",":
											comas <- comas + 1
										Caso ".":
											puntos <- puntos + 1
										Caso ";":
											puntoYComa <- puntoYComa + 1
										Caso ":":
											dosPuntos <- dosPuntos + 1
									FinSegun
								FinPara
								
								Escribir "Cantidad de comas: ", comas
								Escribir "Cantidad de puntos: ", puntos
								Escribir "Cantidad de punto y coma: ", puntoYComa
								Escribir "Cantidad de dos puntos: ", dosPuntos
						18:
								Definir cadena Como Cadena
								Definir vocales, consonantes, digitos Como Entero
								
								Escribir "Ingrese una cadena de texto: "
								Leer cadena
								
								vocales <- 0
								consonantes <- 0
								digitos <- 0
								
								Para i <- 0 Hasta Longitud(cadena) - 1 Hacer
									car <- Subcadena(cadena, i, i)
									Si car >= "a" Y car <= "z" O car >= "A" Y car <= "Z" Entonces
										Si car = "a" O car = "e" O car = "i" O car = "o" O car = "u" O car = "A" O car = "E" O car = "I" O car = "O" O car = "U" Entonces
											vocales <- vocales + 1
										Sino
											consonantes <- consonantes + 1
										FinSi
									SiNo
										Si car >= "0" Y car <= "9" Entonces
											digitos <- digitos + 1
										FinSi
									FinSi
								FinPara
								
								Escribir "Cantidad de vocales: ", vocales
								Escribir "Cantidad de consonantes: ", consonantes
								Escribir "Cantidad de dígitos: ", digitos
						19:
								Definir frase Como Cadena
								Definir cantidadPalabras, i Como Entero
								Definir esUnaPalabra Como Logico
								
								Escribir "Ingrese una frase: "
								Leer frase
								
								cantidadPalabras <- 0
								esUnaPalabra <- Falso
								
								Para i <- 0 Hasta Longitud(frase) Hacer
									Si Subcadena(frase, i, i) <> " " Entonces
										Si esUnaPalabra = Falso Entonces
											cantidadPalabras <- cantidadPalabras + 1
											esUnaPalabra <- Verdadero
										FinSi
									Sino
										esUnaPalabra <- Falso
									FinSi
								FinPara
								
								Escribir "La cantidad de palabras en la frase es: ", cantidadPalabras
						20:
								Definir cedula Como Caracter
								Definir sumaDigitos, i Como Entero
								
								Escribir "Ingrese el número de cédula: "
								Leer cedula
								
								sumaDigitos <- 0
								
								Para i <- 0 Hasta Longitud(cedula) - 1 Hacer
									sumaDigitos <- sumaDigitos + ConvertirANumero(Subcadena(cedula, i, i))
								FinPara
								
								Escribir "La suma de los dígitos de la cédula ", cedula, " es: ", sumaDigitos
						21:
								Definir palabra, inversa Como Cadena
								Definir i, long Como Entero
								
								Escribir "Ingrese una palabra: "
								Leer palabra
								
								long <- Longitud(palabra)
								
								Para i <- long hasta 1 hacer
									inversa <- concatenar(inversa, Subcadena(palabra, i, i))
								Fin Para
								
								Si palabra = inversa entonces
									Escribir "La palabra es palíndromo."
								Sino
									Escribir "La palabra no es palíndromo."
								Fin Si
					FinSegun
				Hasta Que opcion = 21
			3:
				Escribir "¡Hasta luego!"
			De Otro Modo:
				Escribir "Opción inválida. Intente nuevamente."
		FinSegun
	Hasta Que opcion = 3
FinAlgoritmo

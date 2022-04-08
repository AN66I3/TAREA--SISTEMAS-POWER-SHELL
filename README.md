# TAREA--SISTEMAS-POWER-SHELL
Practica de Powershell. Analizar y documenta los siguientes scripts de Powershell

# En esta práctica nos introducimos en el mundo de

# EJERCICIO 1
#### Se ingresa por consola, se asigna variables y se imprime los números almacenados en cada variable

![image](https://user-images.githubusercontent.com/91564729/162446011-8b113df1-adee-4e4b-b9e8-3f46226e6660.png)

# EJERCICIO 2

# Each time around the loop the code in the brackets will run while $counter is less than than $repeat.
# Each time around the loop the ++ symbols tell the variable to increment by one each time.
[int]$repeat = 5

for ($counter = 0; $counter -lt $repeat; $counter++) {
    Write-Host "hello"
}
#### Se inserta un bucle For mediante un contador que se detendrá al llegar a 5, imprimiendo la palabra "hello". Coloca la expresión (-lt) debido a que el cero también se cuenta 
![image](https://user-images.githubusercontent.com/91564729/162471559-123fa0b3-705c-4866-b18e-9d9645803d4f.png)


#The while loop will continue until $counter is less than (-lt) the value 5 held in the $repeat variable.
[int]$repeat = 5
[int]$counter = 0

while ($counter -lt $repeat) {
    Write-Host "hello"
    $counter++
}
#### Se inserta un bucle indeterminado, mientras , que imprime la palabra "hello" , "mientras  el contador sea igual a longitud -1, es decir del 0 al 5, menos 1.
![image](https://user-images.githubusercontent.com/91564729/162534360-5f145f52-92fd-4875-be35-0adf5c215fa6.png)


# Do While Loop is a variant of the while loop except the code is executed before the condition is checked to see if it repeats.
[int]$repeat = 5
[int]$counter = 0
do {
    Write-Host "hello"
    $counter++
}
while ($counter -lt $repeat) 

En este caso, el código se ejecuta primero y luego se realiza la comprobación
![image](https://user-images.githubusercontent.com/91564729/162534828-92885546-c86e-421b-a9de-8d3ba57c723c.png)


# ForEach Loop
# Each time around the loop the $character variable becomes the next character in the list until there are no characters left.
[string]$stringOfCharacters = "PowerShell for Beginners"

foreach ($character in $stringOfCharacters.ToCharArray()) {
    Write-Host $character
} 
Estos comandos imprimen un caracter en cada línea
![image](https://user-images.githubusercontent.com/91564729/162535209-a304d700-dc8e-48d0-9709-e576ef0efa8a.png)


# ForEach-Object loops
[string]$stringOfCharacters = "PowerShell for Beginners"
$stringOfCharacters.ToCharArray() | ForEach-Object { Write-Host "$_" }

Imprime un array saltando línea, para cada objeto
![image](https://user-images.githubusercontent.com/91564729/162535586-dba78a7f-1fca-43cd-8812-5131725152c0.png)

#EJERCICIO 3

####1
![image](https://user-images.githubusercontent.com/91564729/162535918-7ae472d9-526d-4324-9c6f-fade0c175813.png)
#### 2
![image](https://user-images.githubusercontent.com/91564729/162535999-38ab4074-0e05-45ec-8573-5d3448a6de25.png)
#### 3
![image](https://user-images.githubusercontent.com/91564729/162536125-e0110668-cfd2-49e3-b7b2-cabd657dfd04.png)
#### 4 , 5
![image](https://user-images.githubusercontent.com/91564729/162536205-a8528340-6c37-4f2f-967c-1174bc61dc9c.png)
##### 6, 7, 8, 9, 10
![image](https://user-images.githubusercontent.com/91564729/162536310-e08f6160-286b-471a-a3d1-a993617c3c29.png)
##### like y no like

![image](https://user-images.githubusercontent.com/91564729/162536427-f211c91b-c5f4-4146-bb4d-f88a5ed7bbcb.png)
#### match y no match
![image](https://user-images.githubusercontent.com/91564729/162536502-424ce134-e3e2-4b84-92c3-a529cba5d046.png)

#### contens and no contens

![image](https://user-images.githubusercontent.com/91564729/162536617-f284c54f-9897-49db-96ef-f7514c2882b6.png)

#### is and not in
![image](https://user-images.githubusercontent.com/91564729/162536688-53172558-afcb-46d9-aab1-592b5d8de782.png)


### sentencia switch - se usa para variedad de opciones.
![image](https://user-images.githubusercontent.com/91564729/162536817-037424c0-fec7-41f6-88a3-84c7bdd4ddaf.png)





# Práctica del curso de git, gitHub y Sourcetree

## Ejercicio 1

### ¿Qué comando utilizaste en el paso 11? ¿Por qué?
> `git reset --hard HEAD~1`
> 
> Porque se nos pedía deshacer el último commit perdiendo los cambios realizados en el working copy, si hubiese hecho un `git reset HEAD~1`, no se habrían 'perdido' los cambios.

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
> `git reflog`
> 
> `git reset --hard numerodecommitanterior`
> 
> Porque el commit estaba 'perdido' por tanto primero usé un `git reflog` para localizar el hash del commit que queriamos rehacer y luego un `git reset --hard numerodecommit` para dehacer lo deshecho.

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
> No fué un conflicto, git me informo con un mensaje `Already up to date` que todos los cambios de la rama que está intentando fusionar ya se han fusionado con la rama en la que se encuentra actualmente.

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
> Si
> 
> Porque hay lineas de codigo con diferente contenido en la misma posición lo que provoca que git no sepa con que contenido quedarse, para soluciuonarlo abriremos el archivo que causó el conflicto y eligiremos con que código debe quedarse GIT. Guardaremos, lo añadiremos y haremos un commit por último. Con estos pasos debería solucionarse el conflicto y ejecutar el merge con éxito. 

### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
> No, ya que con el merge actualizamos la rama master al punto donde estaba styled.

### ¿Qué comando o comandos utilizaste en el paso 25?
> `git log --graph --decorate --pretty=oneline`

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
> Si, porque al igual que en el merge del paso 21, solo sería actualizar una rama con nuevo contenido. 

### ¿Qué comando o comandos utilizaste en el paso 27?
> `git reset HEAD~1`

### ¿Qué comando o comandos utilizaste en el paso 28?
> `git restore git-nuestro.md`

### ¿Qué comando o comandos utilizaste en el paso 29?
> `git branch -D title`

### ¿Qué comando o comandos utilizaste en el paso 30?
> `git reflog`
> 
> `git reset --hard numerodecommit`

### ¿Qué comando o comandos usaste en el paso 32?
> `git reset numerodecommit`
> 
> Con el `git reflog` del paso 30 ya tenía los números de commit para el paso 32 y 33

### ¿Qué comando o comandos usaste en el punto 33?
> `git reset numerodecommit`
> 
> Con el `git reflog` del paso 30 ya tenía los números de commit para el paso 32 y 33

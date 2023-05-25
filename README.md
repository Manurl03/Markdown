# 1. Taller de Introducción a Markdown
## 1.1 ¿Qué es Markdown? 
[Markdown](https://daringfireball.net/projects/markdown/) es un lenguaje de marcado ligero creado por [John Gruber](https://en.wikipedia.org/wiki/John_Gruber) y [Aaron Swartz](https://es.wikipedia.org/wiki/Aaron_Swartz) que trata de **facilitar la redacción y lectura de documentos en texto plano**, utilizando un conjunto de etiquetas muy sencillas para aplicar estilo al documento.  

Actualmente no existe un estándar para **Markdown**, por este motivo existen diferentes versiones o flavors de **Markdown**.  

En este curso vamos a trabajar con el flavor que se utiliza en GitHub para redactar los archivos README.md de los repositorios y la documentación técnica de los proyectos. Además *GitHub*, junto a *Discourse* o *reddit* están llevando una iniciativa para crear un estándar moderno de **Markdown** como es **CommonMark**.  

En plataformas de repositorios remotos como *GitHub*, la función de este archivo es presentar información del proyecto, como:  

<ul>
  <li> Descripción de su proyecto </li>
  <li> Funcionalidades </li>
  <li> Cómo pueden usarlo los usuarios </li>
  <li> Donde los usuarios pueden encontrar ayuda sobre su proyecto </li>
  <li> Autores del proyecto </li>
</ul>  

## 1.2 Etiquetas básicas de Markdown
### 1.2.1 Encabezados  

**Sintaxis Markdown:**  

```
# Esto es un encabezado h1
## Esto es un encabezado h2
### Esto es un encabezado h3
#### Esto es un encabezado h4
##### Esto es un encabezado h5
###### Esto es un encabezado h6
```  

**HTML renderizado en GitHub:**  
# Esto es un encabezado h1
## Esto es un encabezado h2
### Esto es un encabezado h3
#### Esto es un encabezado h4
##### Esto es un encabezado h5
###### Esto es un encabezado h6
### 1.2.2 Negrita y cursiva  

| Estilo | Métodos abreviados | Sintaxis | Ejemplo | Salida |
| --- | --- | --- | --- | --- | 
| Negrita | `Command+B` (Mac) o `Ctrl+B` (Windows/Linux) | \*\* \*\* o \_\_ \_\_ | \*\*Texto en negrita\*\* | **Texto en negrita** |
| Cursiva | `Command+I` (Mac) o `Ctrl+I`  (Windows/Linux) | \* \* o \_ \_ | \*Texto en cursiva\* | *Texto en cursiva* |
| Tachado | Ninguno | \~\~ \~\~ | \~\~Texto tachado\~\~ | ~~Texto tachado~~ |  

### 1.2.3 Resaltar un comando
**Sintaxis Markdown:**  
En esta frase estamos resaltando el comando \`ls -la\`  
**HTML renderizado en GitHub**  
En esta frase estamos resaltando el comando `ls -la`  

### 1.2.4 Bloques de código  

Al inicio del bloque se puede indicar de forma opcional cuál es el tipo de contenido
que contiene el bloque para resaltar las palabras reservadas cuando se renderice.
Por ejemplo: `bash , python , yaml , json , html , javascript` , etc.  
> Para omitir las comillas triple de bloque (```), podemos albergar todo el bloque
con cuatro comillas (````), o escapar a cada comilla con (\`).  
**Sintaxis Markdown**  
```` 
```
sudo systemctl start apache2
```
````  

```` 
```bash
#!/bin/bash
echo "Hola mundo"
```
````  

```` 
```python
celsius = float(input('Introduce una temperatura en grados
Celsius: '))
farenheit = (1.8 * celsius) + 32
print(f'La temperatura en grados Farenheit es: {farenheit}')
```
````  

**HTML renderizado en GitHub**  

```
sudo systemctl start apache2
```  

```bash
#!/bin/bash
echo "Hola mundo"
```  

```python
celsius = float(input('Introduce una temperatura en grados
Celsius: '))
farenheit = (1.8 * celsius) + 32
print
```  

### 1.2.6 Imágenes  

**Sintaxis Markdown**  

```
Markdown:
![imagen1](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen")
```  

```html
HTML:
<p align="center">
<img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR
</p>
```  

El siguiente código es erróneo, pero se ha introducido para comprobar que aparece
la identificación indicada entre corchetes [imagen3].  

```
Markdown:
![imagen3](/images/instituto.jpeg)
```  
> El error, está en que el nombre del archivo que hay dentro de la carpeta
"images" es "instituto.jpg".  
**HTML renderizado en GitHub:**  

![imagen1](https://pro.iesdonana.org/assets/logo.png "Leyenda de la imagen")  

<p align="center">
<img src="https://pro.iesdonana.org/assets/logo.png" alt="JuveR" width="100px">
</p>  
                                                          
![imagen3](/images/instituto.jpeg)  
                                                          
#### 1.2.7.2 Listas desordenadas anidadas  
                                                          
                                                          

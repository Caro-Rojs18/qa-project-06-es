

# Qa-project-06

E**ste proyecto busca iniciar la automatizacion para sustituir el proceso manual que se han estado utilizando los sprint 
anteriores.
En este sprint, se practica  la automatización de los casos de prueba con el lenguaje de programación Python.


## **por que es importante?**

⏳ La automatización acelera las pruebas. A veces, el proceso de prueba se puede reducir de una semana a una hora. 

⚙️ Hay menos rutina. Puedes liberar tiempo para hacer tareas más interesantes o estudiar nuevas tecnologías.

⛔️ Se reduce el riesgo de error. Los programas informáticos no se cansan ni se distraen.

🤖 La programación se realiza en entornos de desarrollo integrados que admiten el lenguaje de programación requerido. Un ejemplo de un IDE es PyCharm.

🐞 Los y las testers pueden automatizar las pruebas de regresión con Python, JavaScript o algún otro lenguaje de programación.

🔥 Para llevar la aplicación a producción, primero debes configurar las herramientas para el ensamblaje y el despliegue. Esto se puede hacer con herramientas como Jenkins.

##### En este protecto conociendo  La interfaz de PyCharm, y para realizar los testcase Pytest en PyCharm, Pytest  reconoce las pruebas basándose en un prefijo específico. Las funciones que comienzan con test (en minúsculas) son tratadas como pruebas.

# **_PROPOSITO_**

Urban Grocers para  el espacio **name** en la #solicitud de creacion de un kit de productos!

### Acerca del proyecto 

Para iniciar se debe conocer la documentacion para iniciar el ejercicio de automatizacio de la lista de comprobacion 

Urban Grocers Documentation API: https://cnt-2cb651cb-2d3a-42a8-bafd-281348aa0aa2.containerhub.tripleten-services.com/docs/

  
![Image (3).png](..%2F..%2F..%2FDownloads%2FImage%20%283%29.png)





## Se inicia 
### La librería de solicitudes de Python: solicitudes POST

Desde Python Packages se puede acceder a las funciones de la libreria requests que nos permitirá gestionar las solicitudes HTTP de manera sencilla.

Para usar la librería requests en PyCharm (o en cualquier otro entorno de desarrollo), primero debes asegurarte de que está instalada. 

Puedes instalarla fácilmente utilizando pip, el gestor de paquetes de Python. Abre una terminal y ejecuta el siguiente comando:

`pip install requests`

Una vez que la librería esté instalada, Se puede  importar los scripts de Python y comenzar a utilizarla para realizar solicitudes HTTP. Ejemplo básico de cómo puedes usar la 
librería requests para hacer una solicitud GET a una URL:

`import requests

#Hacer una solicitud GET a una URL
response = requests.get('https://api.example.com/data')

#Verificar si la solicitud fue exitosa (código de estado 200)
if response.status_code == 200:`


El proyecto esta organizado con-------Configuración de la ruta
                                      Datos de la solicitud
                                      Importación de datos
                                      Envío de la solicitud POST

vamos con la solicitud POST para crear un kit iniciando con el usuario 

`def post_new_user(body):
    return requests.post(
        configuration.URL_SERVICE + configuration.CREATE_USER_PATH,
        json=body,
        headers=data.headers,
    )
response = post_new_user(data.user_body)`

Uso de Pytest instalando la funcion en Python packages, facilita la escritura de pruebas simples y escalables. 

`pip install pytest`

Es común organizar tus pruebas en un directorio llamado tests en el directorio raíz de tu proyecto. Dentro de 
este directorio, puedes tener archivos de prueba individuales, cada uno conteniendo múltiples funciones de prueba,
o incluso subdirectorios adicionales para organizar mejor tus pruebas.

para ejecutar con Paytest se utiliza el comando `pytest folder/del/proyecto en la terminal`



### Principios Fundamentales


Para que tus pruebas automatizadas sean efectivas y fáciles de mantener, es crucial seguir ciertos principios:

Unidad de comprobación. Cada prueba debe centrarse en una única funcionalidad o aspecto. Esto facilita la identificación de problemas y la corrección de errores.

Independencia de datos. Evita depender de datos específicos que puedan cambiar con el tiempo. En su lugar, genera o utiliza datos que sean consistentes para la prueba.

Autonomía de las pruebas. Cada prueba debe ser capaz de ejecutarse de forma independiente, sin depender del resultado de otras pruebas.

De esta  manera le damos lugar a la creacion de **Autotest**

### Tenemos TEST en este proyecto como

Positive_assert comprueba si el código de estado (status_code) de la respuesta es igual al código de estado esperado y si el nombre (name) devuelto en la respuesta coincide con el nombre esperado.

Negative_assert comprueba si el código de estado (status_code) de la respuesta es igual al código de estado esperado, sin realizar comprobaciones adicionales sobre el cuerpo de la respuesta.**

Archivos especiales de proyectos: gitignore y README

Durante el desarrollo de este proyecto se puede conocer la importancia de la linea de comandos que permita la claridad en los test cases que se realizaron 

### Referencia teorica y caracteristicas 

Documentación oficial de Python https://docs.python.org/es/3/tutorial/index.html
Descarga su última versión desde el sitio web oficial: https://www.python.org/downloads/.
Ficha guia de PyCharm https://practicum-content.s3.us-west-1.amazonaws.com/new-markets/qa-sprint-6/ESP/Atajos_de_teclado_de_PyCharm.pdf
La documentación de Pytest (contenido en inglés) https://docs.pytest.org/en/7.1.x/contents.html
 Git, el sistema de control de versiones más popular (materiales en inglés) https://survey.stackoverflow.co/2021#section-most-popular-technologies-other-tools
Descarga GIT https://git-scm.com/download/
Documentos de GitHub.https://docs.github.com/es/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens

AUTOR 
CAROLINA ROJAS ARCE
SPRINT 6 COHORTE 8
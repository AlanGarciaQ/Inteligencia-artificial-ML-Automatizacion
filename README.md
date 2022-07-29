# Inteligencia artificial: ML Automatización
**Objetivo:** Crear un proceso de aprendizaje automático automatizado.    

![](/imagenes/ml_azure.%20.png)

**Requisitos**
- Cuenta de Azure con una suscripción activa
- Equipo de cómputo con sistema operativo: Windows, Linux o MacOs.  

**Pasos**  
Ingresamos a la página de ml.Azure.com e iniciamos sesión.  
Seleccionamos la opción de crear un área de trabajo.  
En la ventana que se abrió del lado derecho llamada Crear un área de trabajo nueva llenamos los siguientes datos:  
Nombre del área de trabajo: Colocamos queramos que se llame el área de trabajo.  
Suscripción: La suscripción que queramos usar.  
Grupo de recursos: Podemos crear uno o seleccionar uno ya existente.  
Región: Podemos escoger cualquiera, pero si no queremos que haya mucha latencia escogemos uno cercano a donde vivimos.

Para terminar, damos clic en crear.  
![Imagen 1](/imagenes/Imagen1.png)

Damos clic en ir a área de trabajo del área que acabamos de crear.  
En el menú de la izquierda seleccionamos proceso.  
En la pestaña de instancia de proceso seleccionamos nuevo.

**En creación de instancia de proceso, llenamos los siguiente:**  
Nombre del proceso: Colocamos el que queramos.  
Ubicación: Podemos escoger cualquiera.  
Tipo de maquina virtual: Seleccionamos la que prefiramos.   
Tamaño de la maquina virtual: Seleccionamos el que queramos.  
Para terminar, le damos en crear.  
Nota: Instancia de proceso es una forma de decir máquina virtual.  
![](/imagenes/Imagen2.png)

Cuando se termine de crear nuestra instancia de proceso, en el menú de la izquierda volvemos a seleccionar proceso.  
En el apartado de clústeres de proceso seleccionamos nuevo.

**En creación de clústeres de proceso: máquina virtual llenamos lo siguiente:**  
Ubicación: La que queramos.  
Nivel de máquina virtual: Seleccionamos delicado.  
Tipo de máquina virtual: Seleccionamos CPU.  
Tamaño de la maquina virtual: Seleccionamos el que queramos o necesitemos.

Le damos clic en siguiente.  
![](/imagenes/Imagen3.png)

**En creación de clústeres de proceso: Configuración avanzada llenamos lo siguiente:**  
Nombre del proceso: Ponemos el nombre que queramos.  
Número mínimo de nodos: 0  
Número máximo de nodos: 2 (Si se pueden poner más nodos se agregan).  
Lo demás lo dejamos como esta y le damos clic en crear.  
![](/imagenes/Imagen4.png)

Cuando se termine de crear nuestro clúster de proceso, en el menú de la izquierda seleccionamos datos.  
En la pestaña de recursos de datos registrados seleccionamos nuevo y de ahí seleccionamos la opción de archivo web.  
![](/imagenes/Imagen5.png)

En URL pegamos el siguiente link:  https://aka.ms/bike-rentals, los demás datos los llenamos como se ven en siguiente imagen, y le damos a siguiente.  
![](/imagenes/Imagen6.png)

En la siguiente ventana que aparece dejamos todo como esta, solo en el apartado de encabezado de columnas seleccionamos la opción de solo el primer archivo tiene encabezados y le damos clic en siguiente.

En la siguiente ventana seleccionamos todas las opciones, excepto la de Path y le damos a siguiente.  
![](/imagenes/Imagen7.png)

En la siguiente ventana checamos que todos los datos estén bien y le damos en crear.  
A continuación, seleccionamos del menú de la izquierda, la opción de ML automatizado.  
Seleccionamos nuevo trabajo de Ml automatizado.  
En el apartado de Nombre del recurso de datos seleccionamos el que acabamos de crear y le damos a siguiente.  
![](/imagenes/Imagen8.png)

**En Crear un nuevo trabajo de ML automatizado, llenamos lo siguiente:**  
Nombre del experimento nuevo: Colocamos el nombre que queramos que tenga.  
Columna de destino: Seleccionamos la opción de rentals (Integer).  
Seleccionar un tipo de proceso: Seleccionamos Clúster de proceso.  
Seleccionar clúster de proceso de Azure ML: Seleccionamos el clúster que hicimos.  
Damos clic en siguiente.  
![](/imagenes/Imagen9.png)

En la siguiente ventana seleccionamos la opción de regresión y le damos siguiente.  
En la siguiente ventana la dejamos como esta y le damos finalizar.  
Esperamos a que termine el proceso.  
![](/imagenes/Imagen10.png)

Con esto hemos terminado de crear un proceso de aprendizaje automático automatizado.  
![](/imagenes/Imagen11.png)
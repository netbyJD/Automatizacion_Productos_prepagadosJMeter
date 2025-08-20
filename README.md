# Proyecto Postman y JMeter.
Este repositorio contiene las colecciones y entornos de Postman asi como también las automatizaciones/scripts de prueba creados con [Apache JMeter](https://jmeter.apache.org/) para el proyecto de **Consulta de productos y Referidos Prepagados**. A continuación encontrarás las instrucciones para instalar JMeter, importar las colecciones y entornos de Postman, clonar este repositorio, y ejecutar las pruebas localmente.
##Bienvenidos a todos.
## Postman

### ⬇️ Importar la colección
1. Abrir Postman.
2. Hacer clic en **Import**.
3. Seleccionar `collections/VENTA PRODUCTOS SIMA.postman_collection.json`.

### ⬇️ Importar el entorno
1. Hacer clic en **Enviroments** -> **Import**.
2. Seleccionar `enviroments/SERVICIOS.postman_environment.json`.

## JMeter

### 🔧 Requisitos

- Java (JDK) 8 o superior
- Apache JMeter 5.5 o superior
- Git

### 🚀 Instalación de Apache JMeter

1. **Verifica que Java esté instalado:**

```bash
java -version
```

2. **Descarga JMeter:**

- https://jmeter.apache.org/download_jmeter.cgi

3. **Descomprime el archivo:**

- Descomprimir el archivo apache-jmeter-5.5.zit o apache-jmeter-5.5.rar en la carpeta raiz de tu disco local C.

### 📥 Clonar el Repositorio
```bash
git clone [https://github.com/tu-usuario/tu-repo-jmeter.git](https://github.com/jonathan-NB/Automatizacio_Productos_prepagadosJMeter.git)
cd tu-repo-jmeter
```

### ▶️ Ejecutar una Prueba
Puedes ejecutar pruebas de JMeter desde la interfaz gráfica (GUI).

**Usar la Interfaz Gráfica**
```bash
jmeter
```
- Luego, desde el menú:

`Archivo > Abrir` y selecciona uno de los archivos `.jmx` en la carpeta donde tienes guardados los archivos.

### 📦 Datos de Prueba
Algunas pruebas usan archivos CSV. Asegúrate de que la ruta del archivo esté correctamente configurada en el elemento `CSV Data Set Config` de tu script `.jmx`.

### 🧪 Buenas Prácticas
- Usa nombres descriptivos para los archivos `.jmx`.

- Guarda los resultados de pruebas en carpetas por fecha o tipo de prueba.

- No incluyas datos sensibles en los archivos CSV o en el repositorio.

- Versiona los archivos `.jmx` para mantener el control de cambios.

### Notas
- Si el repositorio donde trabajas no es privado no subir los entornos reales con las credenciales, sino solamente subir una plantilla de ejemplo donde tendran que cambiar los valores figticios por los realies para su uso
- Versionar los cambios tanto de las colecciones como de los entornos usando Git desde consola (linea de comandos)

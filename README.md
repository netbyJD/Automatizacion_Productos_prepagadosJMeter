# Proyecto Postman y JMeter
Este repositorio contiene las colecciones y entornos de Postman asi como también las automatizaciones/scripts de prueba creados con [Apache JMeter](https://jmeter.apache.org/) para el proyecto de **Consulta de productos y Referidos Prepagados**. A continuación encontrarás las instrucciones para instalar JMeter, importar las colecciones y entornos de Postman, clonar este repositorio, y ejecutar las pruebas localmente.

## Postman

### Importar la colección
1. Abrir Postman.
2. Hacer clic en **Import**.
3. Seleccionar `collections/VENTA PRODUCTOS SIMA.postman_collection.json`.

### Importar el entorno
1. Hacer clic en **Enviroments** -> **Import**.
2. Seleccionar `enviroments/SERVICIOS.postman_environment.json`.

## JMeter

### 🔧 Requisitos

- Java (JDK) 8 o superior
- Apache JMeter 5.5 o superior
- Git

---

### 🚀 Instalación de Apache JMeter

1. **Verifica que Java esté instalado:**

```bash
java -version
Descarga JMeter:

https://jmeter.apache.org/download_jmeter.cgi

Descomprime el archivo:

bash
Copiar código
tar -xvzf apache-jmeter-5.5.tgz
Agrega JMeter al PATH (opcional):

bash
Copiar código
export PATH=$PATH:/ruta/a/apache-jmeter-5.5/bin
📥 Clonar el Repositorio
bash
Copiar código
git clone https://github.com/tu-usuario/tu-repo-jmeter.git
cd tu-repo-jmeter
▶️ Ejecutar una Prueba
Puedes ejecutar pruebas de JMeter desde la interfaz gráfica (GUI) o desde la línea de comandos (modo no-GUI).

Opción 1: Usar la Interfaz Gráfica
bash
Copiar código
jmeter
Luego, desde el menú:

Archivo > Abrir y selecciona uno de los archivos .jmx en la carpeta pruebas/.

Opción 2: Ejecutar en Modo No-GUI (recomendado para ejecución en CI/CD)
bash
Copiar código
jmeter -n -t pruebas/login-test.jmx -l resultados/login-test.jtl -e -o resultados/reporte-login
Parámetros:

-n: modo no-GUI

-t: ruta al archivo .jmx

-l: archivo donde se guardarán los resultados (.jtl)

-e -o: genera un reporte HTML en la carpeta especificada

📦 Datos de Prueba
Algunas pruebas usan archivos CSV ubicados en la carpeta datos/. Asegúrate de que la ruta del archivo esté correctamente configurada en el elemento CSV Data Set Config de tu script .jmx.

🧪 Buenas Prácticas
Usa nombres descriptivos para los archivos .jmx.

Guarda los resultados de pruebas en carpetas por fecha o tipo de prueba.

No incluyas datos sensibles en los archivos CSV o en el repositorio.

Versiona los archivos .jmx para mantener el control de cambios.

🛠️ Contribuciones
¿Quieres contribuir? Por favor, crea una rama o un pull request siguiendo la convención de nombres, por ejemplo:

bash
Copiar código
git checkout -b feature/nueva-prueba-carga
📄 Licencia
MIT License

📬 Contacto
Si tienes dudas o sugerencias, contacta a:

Nombre: [Tu Nombre]

Email: [tu.email@ejemplo.com]

GitHub: @tu-usuario

yaml
Copiar código

---

### Notas
- Si el repositorio donde trabajas no es privado no subir los entornos reales con las credenciales, sino solamente subir una plantilla de ejemplo donde tendran que cambiar los valores figticios por los realies para su uso
- Versionar los cambios tanto de las colecciones como de los entornos usando Git desde consola (linea de comandos)

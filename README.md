# Ejercicio Práctico: Implementación Inicial de PWA en la Web del Hospital
## Descripción
En este ejercicio práctico, se integran características básicas de una PWA(Progressive Web Application) en el proyecto de la web del hospital.

### Creación del manifiesto 
se crea el manifiesto de la aplicación archivo manifest.json ubicado en la carpeta public, definiento aspectos basicos como nombre y descripcion y algunos detalles asociados a temas, colores e iconos (en diferentes tamaños para favorecer la responsividad de la aplicación).
### Registro de un Service Worker Básico
se implementa un servive worker básico, el cual permite que la aplicación funcione en modo offline, ademas, realice precaching de los archivos principales y se verifica que este se encuentra registrado y activado correctamente.
### Implementación de Estrategias de Almacenamiento en Caché
en esta aplicación se implementa la estrategia de caché STALE-WHILE-REVALIDATE, la cual, basicamente va al cache y a red al mismo tiempo, toma la versión más rápida que siempre será la de cache y en cuanto recibe la de red va a actualizar la versión de cache, esta elección se basa es que es una buena estrategia a la hora de mejorar el rendimiento de la aplicación.
### Pruebas de Funcionamiento Offline y Validación con Lighthouse
mediantes las herramientas de desarrollador proporcionadas por Chrome se comprueba el funcionamiento de la aplicacion en modalidad offline, y se realiza un informe mediante la aplicacion Ligthouse, respecto a la version desktop de la aplicación donde los parametros evaluados arrogan en su mayoria una puntuacion superior a 80.

### Visualización del proyecto
Para visualizar este proyecto se necesita que previamente cuentes con la instalación de:
- **Git**: [sitio de descarga] (https://git-scm.com/downloads)
- **Node.js**: [sitio de descarga] (https://nodejs.org/en/download/package-manager)
- **Visual Studio Code**: [sitio de descarga] (https://code.visualstudio.com/download)
  
Una vez que ya cuentes con lo descrito anteriormente, debes clonar este repositorio en una carpeta local, mediante el siguiente comando:
```bash
git clone https://github.com/lorenasotosanmartin/M6_EJ1.git
```
cuando ya este clonado, escribir el siguiente comando en la consola: 
```bash
npm  i
```
y ejecutar el comando, para inicializar el proyecto: 
```bash
npm run dev
```
Finalmente, para visualizar el proyecto en tu navegador debes abrir la url http://localhost:5173/

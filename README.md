# Instalación del Subsistema de Windows para Linux (WSL) y Configuración de Ubuntu como Entorno de Desarrollo Web con Angular.

## 1. Tiempo de duración:
Duración total: Aproximadamente 90 minutos
- Instalación de WSL y Ubuntu: 30 minutos
- Configuración del entorno (Node.js, Angular CLI, Git): 30 minutos
- Creación y ejecución de proyecto Angular: 30 minutos.
  
## 2. Fundamentos:
El Universo Linux en Windows (USL) es como tener un amigo imaginario en tu PC con Windows 10 y más nuevos. Puedes jugar con Linux sin instalar otro sistema operativo ni hacer malabares al arrancar. USL hace fácil usar los trucos, juguetes y mundos de creación de Linux, lo cual ayuda mucho a los genios de la programación, jefes de sistemas y aprendices de computación.

Hay dos opciones curiosas: WSL 1, que es como un traductor de idiomas entre Linux y Windows, y WSL 2, que usa una especie de miniordenador virtual con un corazón Linux de verdad. La segunda opción es más veloz, se lleva mejor con los programas de Linux y se siente casi como estar en Linux de verdad.

## 3. Conocimientos previos:
Para hacer este ejercicio, los estudiantes deben tener:
- Comandos básicos de Linux (navegación, instalaciones de paquetes, sudo).
- Manejo de terminales en Windows.
- Navegador web para ver los resultados del servidor.
- Uso básico de Git y control de versiones.
- Conceptos de desarrollo web (HTML, CSS, JS).
- Fundamentos de Node.js
  
## 5. Objetivos a alcanzar:
- Implementar un entorno de desarrollo Linux dentro de Windows usando WSL.
- Instalar y configurar Ubuntu con herrramientas modernas como: Node.js, Git y Angular CLI.
- Crear y ejecutar una aplicación Angular desde Ubuntu en WSL.
- Visualizar y verificar la correcta ejecución en el navegador local.
  
 ## 6. Equipo necesario:
- Computador con Windows 10 o superior.
- Acceso a internet.
- Terminal de PowerShell o CMD.
- Microsoft Store.
- Ubuntu 20.04 LTS o superior.
- Node.js v16+ instalado en WSL.
- Angular CLI instalado globalmente.
- Navegador web (Chrome, Edge, Firefox).
- Git.

 ## 7. Material de apoyo:
- Documentación oficial de WSL: https://learn.microsoft.com/en-us/windows/wsl/
- Documentación de Ubuntu: https://ubuntu.com/tutorials
- Documentación de Angular CLI: https://angular.io/cli
- Cheat sheet de comandos Linux: https://github.com/LeCoupa/awesome-cheatsheets
    
## 8. Procedimiento:
### Instalación del Subsistema de Windows para Linux (WSL).
El primer paso se observa la ejecución del comando:
```
wsl --install
````
Este comando instala los componentes esenciales para ejecutar Linux en Windows, incluyendo la Plataforma de Máquina Virtual y el Subsistema de Windows para Linux (WSL).
Luego, se utilizó el comando:
```
wsl --list --online
````
Esto muestra una lista de distribuciones de Linux disponibles para instalar, como Ubuntu, Debian, Kali Linux, Oracle Linux y OpenSUSE.

## Evidencia:
<imag![imagen1](https://github.com/user-attachments/assets/eb505a15-71cd-4172-9fef-89d6538fc3a3)

### Instalación de Ubuntu en WSL.
El segundo paso es ejecutar el comando:
```
wsl --install -d Ubuntu
````
Con esto, se inicia la instalación de la distribución Ubuntu en WSL, mostrando su progreso en la terminal.

## Evidencia:
<imag!![imagen 2](https://github.com/user-attachments/assets/f33e49e1-0cf2-4639-bcb6-930f6e8ca347)

### Descarga de Ubuntu desde Microsoft Store.
El tercer paso se muestra el Microsoft Store descargando Ubuntu 20.04.6 LTS. Esta versión es Long Term Support (LTS), lo que garantiza estabilidad y actualizaciones de seguridad por 5 años.

## Evidencia:
<imag!![imagen 3](https://github.com/user-attachments/assets/a52cd0f6-d166-4a26-aac0-b9d1a375f1e9)

### Instalación del Kernel de Linux para WSL.
El cuarto paso se observa la finalización del asistente de instalación del paquete de actualización del kernel de Linux para WSL. La pantalla muestra el mensaje “Completed the Windows Subsystem for Linux Update Setup Wizard”, lo que indica que el proceso se ha completado con éxito.

## Evidencia:
<imag!![imagen 4](https://github.com/user-attachments/assets/779639f0-1898-4f77-9f9f-2026d276fdb2)

### Inicio de Ubuntu en WSL.
El quinto paso se muestra la terminal de Ubuntu 20.04 LTS ejecutándose dentro de WSL en Windows. Se puede observar información relevante del sistema, como:
- La versión del kernel (5.10.16.3-microsoft-standard-WSL2), lo que confirma que se está utilizando WSL 2.
- La carga del sistema y el uso de memoria, que indican un bajo consumo de recursos.
- Un mensaje sugiriendo ejecutar sudo apt update para verificar la disponibilidad de actualizaciones.

## Evidencia:
<imag!![imagen 5](https://github.com/user-attachments/assets/9f51800b-a72e-48b0-9098-185740508817)

### Comandos en la Terminal de Ubuntu.
El sexto paso se observa nuevamente la terminal de Ubuntu dentro de WSL. Se presentan dos aspectos clave:
- Se muestra un mensaje sobre la posibilidad de actualizar WSL utilizando wsl.exe --update, lo que sugiere que el usuario puede mejorar su instalación con las últimas actualizaciones.
- El usuario ha intentado ejecutar un comando con sudo, pero no se alcanza a visualizar cuál es el comando exacto.

## Evidencia:
<imag!![imagen 6](https://github.com/user-attachments/assets/0003a34f-39fc-4b3a-82be-32f71690312d)

<imag!![imagen 6 1](https://github.com/user-attachments/assets/c93d00bf-d4b3-428f-8110-b5c970f7ea7e)

<imag!![imagen 6 2](https://github.com/user-attachments/assets/a8767142-f993-4da9-8812-14d474ae16b5)

### Instalación de Angular CLI.
El séptimopaso se utilizó el siguiente comando para instalar Angular CLI de forma global en el sistema:
```
sudo npm install -g @angular/cli
```
Se verificó la instalación con:
```
ng version
```

## Evidencia:
<imag!![imagen 7](https://github.com/user-attachments/assets/f2ce1c20-1cf9-4f60-b99a-f7c4ed68a4c5)

### Creación de un Proyecto Angular.
El octavo paso se creó un nuevo directorio para el proyecto y se generó un nuevo workspace con el comando:
```
mkdir linux-angular
```
```
cd linux-angular
```
```
ng new linux-angular
```
Durante la configuración, se activó la función de autocompletado para comandos ng. Se eligieron las siguientes opciones:
-Uso de CSS como preprocesador de estilos
-Configuración de Server-Side Rendering (SSR) y Static Site Generation (SSG)

## Evidencia:
<imag!![imagen 8](https://github.com/user-attachments/assets/a76e74ad-caa1-499f-a8c4-c1dd9e7c3f7a)

<imag!![imagen 8 1](https://github.com/user-attachments/assets/20d72346-5875-434a-a6a1-6a1691d779d2)

### Configuración de Git.
El noveno paso es intentar inicializar el repositorio Git, pero surgió un error debido a la falta de identidad del usuario en la configuración global de Git. Para corregirlo, se deben ejecutar los siguientes comandos:
```
git config --global user.email "tu_correo@example.com"
```
```
git config --global user.name "Tu Nombre"
```

## Evidencia:
<imag!![imagen 9](https://github.com/user-attachments/assets/03177a10-577a-4ab6-b9a0-14efe97465b8)

<imag!![imagen 9 1](https://github.com/user-attachments/assets/60138899-d7e7-4c7e-ab6e-8a36bb1ae14e)

## 9. Resultados esperados:
Tras la compilación exitosa, la aplicación Angular se ejecutó correctamente en el puerto 4200 del entorno local. La pantalla de bienvenida de Angular se visualizó en el navegador confirmando que el servidor está funcionando correctamente.

## Evidencia:
<imag!![image](https://github.com/user-attachments/assets/701f5347-e8d5-46fc-9e94-d21520dbcf50)

## 10. Conclusión:
El proceso de instalación de WSL y Ubuntu en Windows es eficiente y accesible, gracias a los comandos integrados de Windows 10 y 11, lo que simplifica la implementación de un entorno Linux dentro de un sistema operativo Windows. WSL ofrece una solución robusta para ejecutar una distribución Linux completa, brindando a los desarrolladores un entorno ideal para tareas de desarrollo web, sin necesidad de recurrir a máquinas virtuales o particiones duales.

La instalación de Angular CLI y la creación de proyectos en este entorno se realizó sin inconvenientes, demostrando que la integración entre Ubuntu en WSL y herramientas de desarrollo como Git y Node.js es fluida. Este entorno mixto de trabajo aprovecha las fortalezas de ambos sistemas operativos, proporcionando una plataforma de desarrollo moderna, flexible y eficiente.

Finalmente, se alcanzó el objetivo de ejecutar una aplicación Angular desde Ubuntu en WSL, lo que confirma que este sistema es perfectamente funcional para desarrollar aplicaciones web y visualizarlas en un navegador, lo que potencia las capacidades de desarrollo en un solo equipo.

  ## 11. Bibliografía:
Microsoft. (2023). Windows Subsystem for Linux documentation. Microsoft Learn. https://learn.microsoft.com/en-us/windows/wsl/

Canonical. (2023). Ubuntu tutorials. Ubuntu. https://ubuntu.com/tutorials

Google. (2023). Angular CLI overview and command reference. Angular. https://angular.io/cli

Torvalds, L. (2003). The Linux command line. No Starch Press.

Docker Inc. (2023). Docker documentation. https://docs.docker.com/

<h1 align="center">
  <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://f.hubspotusercontent20.net/hubfs/2829524/Copia%20de%20LOGOTIPO_original-2.png"></a>
  <br>
  qa-mobile-maestro
  <br>
</h1>

<h4 align="center">Proyecto base de <a href="https://maestro.mobile.dev/getting-started/installing-maestro" target="_blank">Pragma</a>.</h4>


<p align="center">
  <a href="https://ubuntu.com/desktop/wsl">
   <img alt="Ubuntu" src="https://img.shields.io/badge/WSL-Ubuntu-orange">
  </a>

  <a href="https://maestro.mobile.dev/getting-started/installing-maestro">
   <img alt="Maestro" src="https://img.shields.io/badge/Maestro-Mobile_Testing-white">
  </a>
  
  <a href="https://developer.android.com/studio?hl=es-419">
   <img alt="Android Studio" src="https://img.shields.io/badge/Android_Studio-Emulator-blue">

  </a>
  
</p>

Este repositorio contiene un proyecto de automatización de pruebas para aplicaciones móviles utilizando Maestro, 
una herramienta de código abierto para la automatización de flujos de trabajo en dispositivos móviles. 
Maestro permite realizar pruebas funcionales y de interfaz de usuario de manera eficiente y sencilla en aplicaciones Android e iOS.

<p align="center">
  <a href="#topicos">Topicos</a> •
  <a href="#tecnologias">Tecnologias</a> •
  <a href="#consideraciones">Consideraciones</a> •
  <a href="#descarga">Descarga</a> •
  <a href="#instalación-y-ejecución">Instalación y ejecución</a> •
  <a href="#autores">Autores</a> •
  <a href="#relacionados">Relacionados</a> •
  <a href="#roadmap">Roadmap</a>
</p>

![screenshot](images/maestro.gif)

## Topicos

* Yaml
* Ubuntu
* Maestro
* Javascript
* Android

## Tecnologias
### This project required:
- [JDK java] version 11
- [wsl] Ubuntu 22.04.4
- [maestro] last version

Nota: 
*   Es necesario tener un dispositivo móvil físico (Android) o un emulador/simulador (Android/IOS) configurado correctamente.
  
## Consideraciones
- Para hacer uso de la la utilidad de Base de Datos es importante 
        que se instacie una Base de datos y se configura en el archivo de configuración ubicado en:

            ./src/main/resources/configs/congig.properties

        En las dependencias del proyecto esta agregada la dependencia del driver de MySQL, si no 
        desea realizar mayores ajustes respecto al motor de BD use MySQL. Si desea usar otro motor, 
        adiciones la dependencia del driver al build.gradle y configure este driver como observa 
        se realizo para MySQL en: 
    
            ./src/main/java/utils/ConectionBD.java
        
        Nota: Algunos motores de BD no requieren agregar la dependencia del driver como Oracle o MSserver

## Descarga
Para clonar está aplicación desde la linea de comando:

```bash
git clone https://github.com/somospragma/qa-mobile-maestro.git
git remote remove origin
git remote add origin URL_DE_TU_NUEVO_REPOSITORIO
git push -u origin master
```
Nota: Asegúrate de reemplazar URL_DE_TU_NUEVO_REPOSITORIO con la URL del repositorio que creaste en tu cuenta de GitHub.

## Instalación y ejecución

Para ejecutar está aplicación, necesitas [Maestro](https://maestro.mobile.dev/getting-started/installing-maestro) y [Ubuntu](https://ubuntu.com/desktop/wsl) instalados en tu equipo.
Desde la linea de comando:

```bash
#Maestro
curl -Ls "https://get.maestro.mobile.dev" | bash

#Wsl - Ubuntu
wsl --install
```

##  🛠️ Run tests:
```
maestro --udid=<nombre-emulador>  --host <ip> test <nombre_archivo_test>.yaml
```

## Autores


| [<img src="https://gitlab.com/uploads/-/system/user/avatar/13437423/avatar.png?width=400" width=115><br><sub>Mauro L. Ibarra P.</sub>](https://gitlab.com/mauro.ibarrap) <br/> | [<img src="https://secure.gravatar.com/avatar/23b2db02403d79ebd356e8e8356758ec?s=192&d=identicon" width=115><br><sub>Otro autor</sub>](https://gitlab.com/) | 
:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|


## Relacionados

- [proyecto-base-serenity-bdd-screenplay-browsers-and-utilities](https://github.com/somospragma/qa-web-proyecto-base-serenity-bdd-screenplay-browsers-and-utilities)


## Roadmap

- [Guia QA](https://github.com/amitmerchant1990/pomolectron) - (En construcción) Una guia de proyectos Orientados a la Calidad de Software


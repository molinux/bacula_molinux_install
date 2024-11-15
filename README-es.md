**Bacula Community Molinux Install** is approved in the following distributions and versions:

| Distro       | Version                        |
|:-------------|:-------------------------------|
| Debian       | 11 (bullseye)                  |
| Oracle Linux | 9.3                            |
| Alma Linux   | AlmaLinux 9.4 (Seafoam Ocelot) |
| Rocky        | Rocky Linux 9.3 (Blue Onyx)    |

<!-- Improved compatibility of volver al inicio link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="./assets/icons8-morcego-96.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">BCMI</h3>

  <p align="center">
    Bacula Community Molinux Install
    <br />
    <a href="https://github.com/molinux/bacula_molinux_install/blob/main/README-pt_BR.md"><strong>Portugês »</strong></a>
    <a href="https://github.com/molinux/bacula_molinux_install/blob/main/README-es.md"><strong>Español »</strong></a>
    <a href="https://github.com/molinux/bacula_molinux_install/blob/main/README-en.md"><strong>English</strong></a>
    <br />
    <br />
    <a href="https://github.com/molinux/bacula_molinux_install/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/molinux/bacula_molinux_install/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## Acerca del Proyecto

[![BCMI Screen Shot][product-screenshot]](https://example.com)

> Bacula Community Molinux Install (BCMI) es la herramienta definitiva que necesitas para instalar tu servidor Bacula Community (y entorno).

---

¿Por qué usarlo?

* Instalación automática con solo unos pocos pasos.
* Posibilidad de instalar componentes aislados (almacenamiento y/o cliente).
* Instalación de Bacula y Bacularis en el mismo lugar.
* Documentación disponible en Portugués, Inglés y Español.

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- GETTING STARTED -->
## Introducción

### Requisitos previos

Para instalar Bacula Community y/o Bacularis usando BCMI, debes crear una cuenta en [bacula.org](https://www.bacula.org/bacula-binary-package-download/) y [bacularis.app](https://users.bacularis.com/user/login/) previamente y obtener tu clave/usuario/contraseña.

Después de esto, introduce esta información en el archivo bacula_molinux_install.conf como en el ejemplo a continuación:

```bash
bacula_key="69549348539sdvsd2623"
bacularis_user="sdfgh98ysdfgsdfg"
bacularis_pass="sdlfgsdfg-WEWERTBsdfsdfg"
```

O puedes especificarlo durante la instalación:

```bash
--------------------------------------------------
 Informe su clave de Bacula
 Esta clave se obtiene con el registro en Bacula.org.
 https://www.bacula.org/bacula-binary-package-download/
 Por favor, introduzca su clave de Bacula:
```

### Instalación

_Sigue los pasos a continuación para instalar y configurar tu aplicación:_

1. Crea tu cuenta en [bacula.org](https://www.bacula.org/bacula-binary-package-download/) y [bacularis.app](https://users.bacularis.com/user/login/)

2. Descarga el archivo de configuración:

```sh
wget https://abre.ai/bacula-molinux-install-conf
```

3. Descarga el archivo de instalación:

```sh
wget https://abre.ai/bacula-molinux-install-app
```

4. Introduce tus credenciales en el archivo `bacula_molinux_install.conf`:

```bash
bacula_key="69549348539sdvsd2623"
bacularis_user="sdfgh98ysdfgsdfg"
bacularis_pass="sdlfgsdfg-WEWERTBsdfsdfg"
```

O puedes especificarlo durante la instalación:

```bash
--------------------------------------------------
 Informe su clave de Bacula
 Esta clave se obtiene con el registro en Bacula.org.
 https://www.bacula.org/bacula-binary-package-download/
 Por favor, introduzca su clave de Bacula:
```

5. Haz que el archivo `bacula_molinux_install-app` sea ejecutable:

```bash
chmod +x bacula_molinux_install-app
```

6. Ejecuta el instalador:

```bash
./bacula_molinux_install-app
```

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- USAGE EXAMPLES -->
## Uso

Después de instalar la aplicación, puedes usar bconsole para conectarse a Bacula Director (servidor)

```bash
bconsole

Connecting to Director localhost:9101
1000 OK: 10002 bacula-dir Version: 15.0.2 (21 March 2024)
Enter a period to cancel a command.
*
```

Y/o configurar Bacularis desde su navegador

[![Bacularis API Screen Shot][bacularis-api-screenshot]](https://example.com)

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- ROADMAP -->
## Roadmap

* [ ] Bacula container version
* [ ] Bacularis container version
* [ ] Multi-language Support
  * [ ] Brazilian Portuguese
  * [ ] Spanish

Consulte los [problemas abiertos](https://github.com/molinux/bacula_molinux_install/issues) para obtener una lista completa de las características propuestas (y los problemas conocidos)

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- CONTRIBUTING -->
<!-- ## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p> -->

<!-- LICENSE
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p> -->

<!-- CONTACT -->
## Contacto

Marcus Molinero - [linkedin](https://linkedin.com/in/marcus-molinero) - <marcus.molinero@bacula.com.br>

Project Link: [Bacula Community Molinux Install](https://github.com/molinux/bacula_molinux_install)

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

## Asociaciones
<!-- <center> -->
<table>
 <tr>
        <td><a href="https://www.bacula.lat"><img src="./assets/Logo-Bacula-Brasil.jpg"></a></td>
        <td><a href="https://www.nomaland.com.br"><img src="./assets/Logo-Nomaland-2.png"></a></td>
 <tr>
</table>
 <!-- </center> -->

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p>

<!-- ACKNOWLEDGMENTS -->
<!-- ## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">volver al inicio</a>)</p> -->

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: assets/bcmi-001.png
[bacularis-api-screenshot]: assets/bcmi-002.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com
[Bash-url]: https://cdn.rawgit.com/odb/official-bash-logo/master/assets/Logos/Identity/PNG/BASH_logo-transparent-bg-color.png

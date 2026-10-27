# .github de Grupo Faro

Repositorio de documentación comunitaria y perfil público de [Grupo Faro](https://grupofaro.es). Reúne las pautas generales de colaboración, accesibilidad, seguridad y soporte de los proyectos de la organización en [GitHub](https://github.com/Grupo-Faro).

Está dirigido a quienes consultan la organización y a las personas que revisan o actualizan sus documentos. Su contenido se mantiene como archivos de texto versionados; es un repositorio documental, sin aplicación ejecutable ni servicios que desplegar.

## Funciones principales

- Documentación de entrada sobre el propósito y la estructura del repositorio.
- Perfil público de organización definido en `profile/README.md`.
- Pautas comunitarias predeterminadas para los proyectos que no tengan documentos propios del mismo tipo.
- Contenidos versionados, consultables y editables como archivos [Markdown](https://commonmark.org/).

## Estructura

| Archivo | Finalidad |
| --- | --- |
| `README.md` | Guía para consultar y mantener este repositorio. |
| [`profile/README.md`](profile/README.md) | Contenido que se muestra en el perfil público de la organización. |
| [`ACCESSIBILITY.md`](ACCESSIBILITY.md) | Prioridades de accesibilidad y comunicación de barreras. |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Normas de convivencia y canales para comunicar incidentes. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Orientaciones para informar de problemas y proponer cambios. |
| [`SECURITY.md`](SECURITY.md) | Comunicación privada y gestión de vulnerabilidades. |
| [`SUPPORT.md`](SUPPORT.md) | Canales y contexto necesario para solicitar ayuda. |
| [`LICENSE.md`](LICENSE.md) | Texto íntegro de la licencia del repositorio. |

El README de la raíz y el del perfil tienen funciones distintas. Modificar este documento no modifica el perfil de la organización. El funcionamiento del perfil se describe en la [documentación oficial de GitHub](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile).

Los documentos comunitarios de este repositorio público pueden utilizarse como valores predeterminados cuando un proyecto no tiene los suyos. No se copian a los clones ni reemplazan instrucciones particulares. La licencia se declara en cada proyecto. Consulta [el funcionamiento de los documentos predeterminados](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

El perfil destinado a miembros se mantiene por separado en un repositorio privado. Este repositorio público contiene únicamente material apto para su consulta pública.

## Stack tecnológico

- [Markdown](https://commonmark.org/) para los documentos.
- [Git](https://git-scm.com/) para el historial de cambios.
- [GitHub](https://github.com/) para alojar el repositorio, mostrar los documentos y revisar propuestas de cambio.

## Requisitos

Para consultar el contenido basta un navegador. Para proponer cambios desde la web se necesita una cuenta con el acceso correspondiente. El trabajo local requiere [Git](https://git-scm.com/) y un editor de texto.

## Preparación desde cero

Clona el repositorio en una carpeta de trabajo:

```sh
git clone https://github.com/Grupo-Faro/.github.git grupo-faro-comunidad
cd grupo-faro-comunidad
```

Abre `README.md` o `profile/README.md` en el editor para consultar sus contenidos. No hay dependencias que instalar, compilación, variables de entorno, base de datos ni servidor de aplicación.

## Actualización y publicación

1. Actualiza la copia local de `main` y crea una rama para el cambio:

   ```sh
   git switch main
   git pull --ff-only origin main
   git switch -c docs/descripcion-del-cambio
   ```

2. Edita el documento correspondiente y comprueba su vista previa. Revisa los enlaces relativos y externos y evita incluir credenciales, datos personales o información de infraestructura privada.
3. Comprueba el cambio antes de confirmarlo:

   ```sh
   git diff --check
   git diff
   ```

4. Confirma los archivos previstos, publica la rama y abre una solicitud de incorporación contra `main`.
5. Una persona mantenedora revisa y fusiona la propuesta. Los cambios del perfil público se publican desde `profile/README.md` en la rama predeterminada; no requieren un despliegue separado.

La comprobación de este repositorio es documental: contenido, enlaces, renderizado y licencia. No contiene una aplicación ni una suite de pruebas funcionales.

## Licencia

Este repositorio se distribuye bajo [GPL (Licencia Pública General de GNU), versión 3.0](https://www.gnu.org/licenses/gpl-3.0.html). El texto íntegro se incluye en [`LICENSE.md`](LICENSE.md).

La licencia se refiere al contenido de este repositorio. Cada proyecto de la organización mantiene su propia licencia; este archivo no modifica las licencias de otros repositorios ni concede derechos sobre marcas o contenidos de terceros enlazados.

## Enlaces

- [Organización Grupo Faro en GitHub](https://github.com/Grupo-Faro).
- [Sitio web de Grupo Faro](https://elfaro.xyz).

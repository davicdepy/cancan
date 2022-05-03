# CanCan

[![Estado de compilación](https://github.com/dfinity/cancan/workflows/CI/badge.svg)](https://github.com/dfinity/cancan/actions)

> Un servicio escalable para compartir videos.

## Instalación

### Requisitos previos

- [SDK de computadora de Internet] (https://sdk.dfinity.org)
- [Node.js](https://nodejs.org)
- [Python](https://www.python.org)
- [vessel@0.6.0](https://github.com/dfinity/vessel/releases/tag/v0.6.0)

Si aún no tiene una vessel, puede instalarla ejecutando un script de instalación incluido en el proyecto:

```shell
$ ./scripts/vessel-install.sh
```
MacOS podría preguntarle si está seguro de que confía en este paquete. Puedes aceptar con seguridad

Vuelva a verificar que tiene [vessel](https://github.com/dfinity/vessel) instalado en la versión 0.6.*, luego clone este repositorio y navegue hasta el directorio `cancan`.


```shell
$ vessel --versión
# buque 0.6.0

$ git clone git@github.com:dfinity/cancan.git
$ cd cancán
```

Inicie una réplica de computadora de Internet local.

```shell
$ dfx inicio
```

Ejecute los siguientes comandos en otra pestaña de terminal en el mismo directorio.

```shell
$ npm ci # <- Esto instala paquetes desde el archivo de bloqueo para mantener la coherencia

$ ./bootstrap.sh
```

Esto desplegará un contenedor local llamado `cancan_ui`. Para abrir el front-end, obtenga la identificación del contenedor de activos ejecutando `dfx canister id cancan_ui`. Luego abra su navegador y vaya a `http://<cancan_ui-canister-id>.localhost:8000/sign-in`.

## Desarrollo front-end

Para ejecutar un servidor de desarrollo con actualización rápida y recarga en caliente, puede usar este comando en el directorio raíz de la aplicación:

```shell
$ npm inicio de ejecución
```

Su navegador predeterminado abrirá (o enfocará) una pestaña en `localhost:3000`, a la que luego debe agregar `/?canisterId=${cancan_ui_canister_id}`, donde `cancan_ui_canister_id` es típicamente (actualmente) `ryjl3-tyaaa- aaaaaa-aaaba-cai`.

Ahora puede realizar cambios en cualquier código de frontend y ver actualizaciones instantáneas, en muchos casos sin siquiera requerir una actualización de la página, por lo que el estado de la interfaz de usuario se conserva entre los cambios. Ocasionalmente, agregar una regla CSS no desencadenará una actualización y el usuario debe actualizar manualmente para ver esos cambios.

## Identidad de Internet localmente

Clone y configure [el proyecto] (https://github.com/dfinity/internet-identity) y asegúrese de que `internet_identity` esté implementado y tenga el front-end disponible. Eso debería permitirle realizar la autenticación localmente para probar el nuevo servicio de identidad de Internet. Para la producción, probablemente configuraremos `identity.ic0.app` para ejecutar este contenedor, pero por ahora esta es la forma de hacerlo funcionar.

## English
# CanCan

[![Build Status](https://github.com/dfinity/cancan/workflows/CI/badge.svg)](https://github.com/dfinity/cancan/actions)

> A scalable video-sharing service.

## Installation

### Prerequisites

- [Internet Computer SDK](https://sdk.dfinity.org)
- [Node.js](https://nodejs.org)
- [Python](https://www.python.org)
- [Vessel@0.6.0](https://github.com/dfinity/vessel/releases/tag/v0.6.0)

If you don't have vessel yet you can install it by running an install script included in the project:

```shell
$ ./scripts/vessel-install.sh
```
MacOS might ask if you're sure you trust this package. You can safely accept

Double-check you have [vessel](https://github.com/dfinity/vessel) installed at version 0.6.*, then clone this repository and navigate to the `cancan` directory.


```shell
$ vessel --version
# vessel 0.6.0

$ git clone git@github.com:dfinity/cancan.git
$ cd cancan
```

Start a local Internet Computer replica.

```shell
$ dfx start
```

Execute the following commands in another terminal tab in the same directory.

```shell
$ npm ci # <- This installs packages from the lockfile for consistency

$ ./bootstrap.sh
```

This will deploy a local canister called `cancan_ui`. To open the front-end, get the asset canister id by running `dfx canister id cancan_ui`. Then open your browser, and navigate to `http://<cancan_ui-canister-id>.localhost:8000/sign-in`.

## Frontend Development

To run a development server with fast refreshing and hot-reloading, you can use this command in the app's root directory:

```shell
$ npm run start
```

Your default browser will open (or focus) a tab at `localhost:3000`, to which you must then append `/?canisterId=${cancan_ui_canister_id}`, where `cancan_ui_canister_id` is typically (at current) `ryjl3-tyaaa-aaaaa-aaaba-cai`.

Now you can make changes to any frontend code and see instant updates, in many cases not even requiring a page refresh, so UI state is preserved between changes. Occasionally adding a CSS rule won't trigger an update, and the user has to manually refresh to see those changes.

## Internet Identity Locally

Clone and setup [the project](https://github.com/dfinity/internet-identity) and make sure that `internet_identity` is deployed, and you have the front-end available. That should allow you to do auth locally to try out the new Internet Identity service. For production, we will probably configure `identity.ic0.app` to be running this canister, but for now this is how to get it running.

## Spanish

# CanCan

[![Estado de compilación](https://github.com/dfinity/cancan/workflows/CI/badge.svg)](https://github.com/dfinity/cancan/actions)

> Un servicio escalable para compartir videos.

## Instalación

### Requisitos previos

- [SDK de computadora de Internet] (https://sdk.dfinity.org)
- [Node.js](https://nodejs.org)
- [Python](https://www.python.org)
- [vessel@0.6.0](https://github.com/dfinity/vessel/releases/tag/v0.6.0)

Si aún no tiene una vessel, puede instalarla ejecutando un script de instalación incluido en el proyecto:

```shell
$ ./scripts/vessel-install.sh
```
MacOS podría preguntarle si está seguro de que confía en este paquete. Puedes aceptar con seguridad

Vuelva a verificar que tiene [vessel](https://github.com/dfinity/vessel) instalado en la versión 0.6.*, luego clone este repositorio y navegue hasta el directorio `cancan`.


```shell
$ vessel --versión
# buque 0.6.0

$ git clone git@github.com:dfinity/cancan.git
$ cd cancán
```

Inicie una réplica de computadora de Internet local.

```shell
$ dfx inicio
```

Ejecute los siguientes comandos en otra pestaña de terminal en el mismo directorio.

```shell
$ npm ci # <- Esto instala paquetes desde el archivo de bloqueo para mantener la coherencia

$ ./bootstrap.sh
```

Esto desplegará un contenedor local llamado `cancan_ui`. Para abrir el front-end, obtenga la identificación del contenedor de activos ejecutando `dfx canister id cancan_ui`. Luego abra su navegador y vaya a `http://<cancan_ui-canister-id>.localhost:8000/sign-in`.

## Desarrollo front-end

Para ejecutar un servidor de desarrollo con actualización rápida y recarga en caliente, puede usar este comando en el directorio raíz de la aplicación:

```shell
$ npm inicio de ejecución
```

Su navegador predeterminado abrirá (o enfocará) una pestaña en `localhost:3000`, a la que luego debe agregar `/?canisterId=${cancan_ui_canister_id}`, donde `cancan_ui_canister_id` es típicamente (actualmente) `ryjl3-tyaaa- aaaaaa-aaaba-cai`.

Ahora puede realizar cambios en cualquier código de frontend y ver actualizaciones instantáneas, en muchos casos sin siquiera requerir una actualización de la página, por lo que el estado de la interfaz de usuario se conserva entre los cambios. Ocasionalmente, agregar una regla CSS no desencadenará una actualización y el usuario debe actualizar manualmente para ver esos cambios.

## Identidad de Internet localmente

Clone y configure [el proyecto] (https://github.com/dfinity/internet-identity) y asegúrese de que `internet_identity` esté implementado y tenga el front-end disponible. Eso debería permitirle realizar la autenticación localmente para probar el nuevo servicio de identidad de Internet. Para la producción, probablemente configuraremos `identity.ic0.app` para ejecutar este contenedor, pero por ahora esta es la forma de hacerlo funcionar.
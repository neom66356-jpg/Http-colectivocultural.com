# Configurar la visibilidad de un repositorio

Puedes elegir quién puede ver tu repositorio.

## Acerca de los cambios a la visibilidad de un repositorio

> \[!NOTE]
> Si no puedes cambiar la visibilidad de un repositorio, es posible que el propietario de la organización haya restringido la posibilidad de cambiar la visibilidad del repositorio solo a los propietarios de la organización. Para más información, consulta [Restringir cambios en la visibilidad de los repositorios en tu organización](/es/organizations/managing-organization-settings/restricting-repository-visibility-changes-in-your-organization).

Te recomendamos revisar las siguientes consideraciones antes de que cambies la visibilidad de un repositorio.

### Convertir un repositorio en privado

* GitHub desasociará las bifurcaciones públicas del repositorio público y las colocará en una red nueva. Las bifurcaciones públicas no se hacen privadas.
* Si utilizas GitHub Free para cuentas personales o de organización, algunas características no estarán disponibles en el repositorio después de que cambies la visibilidad a privada. Cualquier sitio GitHub Pages publicado se despublicará de forma automática. Si agregaste un dominio personalizado al sitio GitHub Pages, deberías eliminar o actualizar tus registros de DNS antes de convertir el repositorio en privado, para evitar el riesgo de una adquisición de dominio. Para más información, consulta [planes de GitHub](/es/get-started/learning-about-github/githubs-plans) y [Administración de un dominio personalizado para el sitio de GitHub Pages](/es/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).
* GitHub ya no incluirá el repositorio en el GitHub Archive Program. Para más información, consulta [Acerca del archivado de contenido y datos en GitHub](/es/repositories/archiving-a-github-repository/about-archiving-content-and-data-on-github#about-the-github-archive-program).
* Características de GitHub Advanced Security, como code scanning, dejarán de funcionar a menos que el repositorio sea propiedad de una organización que tenga acceso a la característica en repositorios privados con una licencia de GitHub Advanced Security, GitHub Code Security o GitHub Secret Protection y suficientes puestos de reserva. Para más información, consulta [Acerca de GitHub Advanced Security](/es/get-started/learning-about-github/about-github-advanced-security).

### Convertir un repositorio en público

* GitHub se desasociará de las bifurcaciones privadas y las convertirá en repositorios privados independientes. Para más información, consulta [¿Qué ocurre con las bifurcaciones cuando se elimina un repositorio o cambia su visibilidad?](/es/pull-requests/collaborating-with-pull-requests/working-with-forks/what-happens-to-forks-when-a-repository-is-deleted-or-changes-visibility#changing-a-private-repository-to-a-public-repository)
* Si va a convertir el repositorio privado en un repositorio público como parte de un movimiento hacia la creación de un proyecto de open source, consulte las guías de [Open Source](http://opensource.guide) para obtener sugerencias e instrucciones útiles. También puede realizar un curso gratuito sobre cómo administrar un proyecto de open source con [GitHub Skills](https://skills.github.com/). Una vez que tu repositorio es público, también puedes ver el perfil de la comunidad de tu repositorio para ver si tu proyecto cumple con las mejoras prácticas para los colaboradores de apoyo. Para más información, consulta [Acerca de los perfiles de comunidad para los repositorios públicos](/es/communities/setting-up-your-project-for-healthy-contributions/about-community-profiles-for-public-repositories).
* El repositorio obtendrá acceso automático a las características de GitHub Advanced Security.
* El historial y los registros de acciones serán visibles para todos los usuarios. Si el repositorio tenía flujos de trabajo reutilizables o necesarios compartidos desde otro repositorio de la organización, la ruta de acceso del archivo de flujo de trabajo, incluido el nombre del repositorio, estará visible en los registros. Para obtener más información sobre cómo eliminar las ejecuciones de flujo de trabajo y los artefactos, consulte [Administrar ejecuciones de flujo de trabajo](/es/actions/managing-workflow-runs#deleting-logs) y [Puntos de conexión de API de REST para ejecuciones de flujo de trabajo](/es/rest/actions/workflow-runs).

Para información sobre cómo mejorar la seguridad del repositorio, consulta [Inicio rápido para proteger el repositorio](/es/code-security/getting-started/securing-your-repository).

## Consecuencias de cambiar la visibilidad de un repositorio

> \[!CAUTION]Antes de cambiar la visibilidad del repositorio, comprenda las consecuencias de este cambio.

### Cambio de público a privado

* Las estrellas y los seguidores de este repositorio se borrarán, lo que afectará a la clasificación del repositorio.
* Las reglas de alertas personalizadas de Dependabot se deshabilitarán a menos que GitHub Code Security esté habilitado para este repositorio. El gráfico de dependencias y las Dependabot alerts permanecerán habilitados con permiso para realizar análisis de solo lectura en este repositorio.

> - Code scanning dejará de estar disponible a menos que Code Security esté habilitado para este repositorio.

* Las bifurcaciones actuales seguirán siendo públicas y se desasociarán de este repositorio.

### Cambio de privado a público

* El código será visible para todos los usuarios que puedan visitar GitHub.com.
* Cualquier persona puede bifurcar su repositorio.
* Todos los conjuntos de reglas de inserción se deshabilitarán.
* Los cambios se publicarán como actividad.
* El historial y los registros de acciones serán visibles para todos los usuarios.
* Se borrarán las estrellas y los monitores de este repositorio.

### Cambio de privado a interno

* A todos los miembros de la empresa se les proporcionará acceso de lectura.
* Los colaboradores externos ya no se pueden agregar a bifurcaciones a menos que se agreguen a la raíz.
* Se borrarán las estrellas y los monitores de este repositorio.

### Cambio de interno a privado

* Las estrellas y los seguidores de este repositorio se borrarán, lo que afectará a la clasificación del repositorio.
* Las reglas de alertas personalizadas de Dependabot se deshabilitarán a menos que GitHub Code Security esté habilitado para este repositorio. El gráfico de dependencias y las Dependabot alerts permanecerán habilitados con permiso para realizar análisis de solo lectura en este repositorio.

> - Code scanning dejará de estar disponible a menos que Code Security esté habilitado para este repositorio.

* Las bifurcaciones actuales seguirán siendo públicas y se desasociarán de este repositorio.

### Cambio de interno a público

* El código será visible para todos los usuarios que puedan visitar GitHub.com.
* Cualquier persona puede bifurcar su repositorio.
* Todos los conjuntos de reglas de inserción se deshabilitarán.
* Los cambios se publicarán como actividad.
* El historial y los registros de acciones serán visibles para todos los usuarios.
* Se borrarán las estrellas y los monitores de este repositorio.

### Cambiar de público a interno

* A todos los miembros de la empresa se les proporcionará acceso de lectura.
* Los colaboradores externos ya no se pueden agregar a bifurcaciones a menos que se agreguen a la raíz.
* Se borrarán las estrellas y los monitores de este repositorio.

## Cambiar la visibilidad de un repositorio

1. En GitHub, navegue hasta la página principal del repositorio.
2. Debajo del nombre del repositorio, haz clic en **<svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-gear" aria-label="gear" role="img"><path d="M8 0a8.2 8.2 0 0 1 .701.031C9.444.095 9.99.645 10.16 1.29l.288 1.107c.018.066.079.158.212.224.231.114.454.243.668.386.123.082.233.09.299.071l1.103-.303c.644-.176 1.392.021 1.82.63.27.385.506.792.704 1.218.315.675.111 1.422-.364 1.891l-.814.806c-.049.048-.098.147-.088.294.016.257.016.515 0 .772-.01.147.038.246.088.294l.814.806c.475.469.679 1.216.364 1.891a7.977 7.977 0 0 1-.704 1.217c-.428.61-1.176.807-1.82.63l-1.102-.302c-.067-.019-.177-.011-.3.071a5.909 5.909 0 0 1-.668.386c-.133.066-.194.158-.211.224l-.29 1.106c-.168.646-.715 1.196-1.458 1.26a8.006 8.006 0 0 1-1.402 0c-.743-.064-1.289-.614-1.458-1.26l-.289-1.106c-.018-.066-.079-.158-.212-.224a5.738 5.738 0 0 1-.668-.386c-.123-.082-.233-.09-.299-.071l-1.103.303c-.644.176-1.392-.021-1.82-.63a8.12 8.12 0 0 1-.704-1.218c-.315-.675-.111-1.422.363-1.891l.815-.806c.05-.048.098-.147.088-.294a6.214 6.214 0 0 1 0-.772c.01-.147-.038-.246-.088-.294l-.815-.806C.635 6.045.431 5.298.746 4.623a7.92 7.92 0 0 1 .704-1.217c.428-.61 1.176-.807 1.82-.63l1.102.302c.067.019.177.011.3-.071.214-.143.437-.272.668-.386.133-.066.194-.158.211-.224l.29-1.106C6.009.645 6.556.095 7.299.03 7.53.01 7.764 0 8 0Zm-.571 1.525c-.036.003-.108.036-.137.146l-.289 1.105c-.147.561-.549.967-.998 1.189-.173.086-.34.183-.5.29-.417.278-.97.423-1.529.27l-1.103-.303c-.109-.03-.175.016-.195.045-.22.312-.412.644-.573.99-.014.031-.021.11.059.19l.815.806c.411.406.562.957.53 1.456a4.709 4.709 0 0 0 0 .582c.032.499-.119 1.05-.53 1.456l-.815.806c-.081.08-.073.159-.059.19.162.346.353.677.573.989.02.03.085.076.195.046l1.102-.303c.56-.153 1.113-.008 1.53.27.161.107.328.204.501.29.447.222.85.629.997 1.189l.289 1.105c.029.109.101.143.137.146a6.6 6.6 0 0 0 1.142 0c.036-.003.108-.036.137-.146l.289-1.105c.147-.561.549-.967.998-1.189.173-.086.34-.183.5-.29.417-.278.97-.423 1.529-.27l1.103.303c.109.029.175-.016.195-.045.22-.313.411-.644.573-.99.014-.031.021-.11-.059-.19l-.815-.806c-.411-.406-.562-.957-.53-1.456a4.709 4.709 0 0 0 0-.582c-.032-.499.119-1.05.53-1.456l.815-.806c.081-.08.073-.159.059-.19a6.464 6.464 0 0 0-.573-.989c-.02-.03-.085-.076-.195-.046l-1.102.303c-.56.153-1.113.008-1.53-.27a4.44 4.44 0 0 0-.501-.29c-.447-.222-.85-.629-.997-1.189l-.289-1.105c-.029-.11-.101-.143-.137-.146a6.6 6.6 0 0 0-1.142 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0ZM9.5 8a1.5 1.5 0 1 0-3.001.001A1.5 1.5 0 0 0 9.5 8Z"></path></svg> Settings**. Si no puedes ver la pestaña "Configuración", selecciona el menú desplegable **<svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-kebab-horizontal" aria-label="More" role="img"><path d="M8 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3ZM1.5 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Zm13 0a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path></svg>** y, a continuación, haz clic en **Configuración**.

   ![Captura de pantalla de un encabezado de repositorio en el que se muestran las pestañas. La pestaña "Configuración" está resaltada con un contorno naranja oscuro.](/assets/images/help/repository/repo-actions-settings.png)
3. En la sección "Zona de peligro", a la derecha de "Cambiar la visibilidad del repositorio", haga clic en **Cambiar visibilidad**.
4. Selecciona una visibilidad.
5. Haga clic para confirmar que está cambiando la visibilidad del repositorio correcto.
6. Haga clic en **He leído y entiendo estos efectos**.
7. Haga clic en **Hacer público este repositorio** o **haga que este repositorio sea privado**.

## Información adicional

* [Acerca de los repositorios](/es/repositories/creating-and-managing-repositories/about-repositories#about-repository-visibility)
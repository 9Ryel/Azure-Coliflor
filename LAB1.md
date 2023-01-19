# LAB 1 - Administración de identidades de Azure Active Directory

Para que los usuarios se puedan autentificar usando Azure AD, debes proveerles con sus usuarios y grupos. La membresía de los grupos debes ser actualizadas automáticamente dependiendo del título de trabajo. Crear un Azure AD tenant con un usuario y darle permisos limitados a los recursos del principal.

Proyecto: [a](./img/99.png)

• Tarea 1: Crear y configurar usuarios en Azure AD.

1- Conectarse a [azure portal](https://portal.azure.com/?l=en.en-us#home).

2- En el portal de azure, buscar y seleccionar Azure Active Directory.

3- En el panel del Azure AD, busca la sección de Manage, dentro de Users y muestra las opciones de configuración.

[a](./img/98.png)

4- Muestra la configuración de perfil de tu cuenta.

[a](./img/97.png)

5- Edita y cambia el Usage Location a United States y guarda el cambio.

[a](./img/96.png)

6- Vuelve a Users y crea un nuevo usuario con los siguientes parámetros:

| Setting                    | Value                     |
|----------------------------|---------------------------|
| User name                  | az104-01a-aaduser1        |
| Name                       | az104-01a-aaduser1        |
| Let me create the password | enabled                   |
| Initial password           | Provide a secure password |
| Usage location             | United States             |
| Job title                  | Cloud Administrator       |
| Department                 | IT                        |

[a](./img/95.png)

7- Añade el rol de User Administrator de Azure AD en el nuevo usuario creado.

[a](./img/94.png)

8- Conecta al portal de azure con el usuario anteriormente creado y entra al Azure AD.

[a](./img/93.png)

9- Con el usuario creado, crea un nuevo usuario con las siguientes parámetros:

| Setting                    | Value                     |
|----------------------------|---------------------------|
| User name                  | az104-01a-aaduser2        |
| Name                       | az104-01a-aaduser2        |
| Let me create the password | enabled                   |
| Initial password           | Provide a secure password |
| Usage location             | United States             |
| Job title                  | System Administrator      |
| Department                 | IT                        |

[a](./img/92.png)

10- Cierra la sesión.

• Tarea 2: Crear grupos de Azure AD con membresía asignada y dinámica.

1- En el panel de Azure AD, busca y entra en Licenses.

2- Dentro de la sección de Manage, en All Products, activa Azure AD premium P2. (Para que se actualicen las membresías automáticamente)

[a](./img/91.png)

> Puede tardar un rato en activarse.

3- Volvamos a Azure AD, y dentro de Groups, creamos uno nuevo con los siguientes parámetros:

| Setting           | Value                           |
|-------------------|---------------------------------|
| Group type        | Security                        |
| Group name        | IT Cloud Administrators         |
| Group description | Contoso IT cloud administrators |
| Membership type   | Dynamic User                    |

[a](./img/90.png)

4- Añadimos una regla en Add dynamic query que indique, jobtitle sea igual a Cloud Administrator.

[a](./img/89.png)

• Tarea 3: Crear un Azure Active Directory (AD) tenant.
• Tarea 4: Administrar invitados en Azure AD.


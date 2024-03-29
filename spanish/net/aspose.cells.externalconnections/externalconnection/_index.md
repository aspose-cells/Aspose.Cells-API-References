---
title: ExternalConnection
second_title: Referencia de API de Aspose.Cells para .NET
description: Especifica una conexión de datos externa
type: docs
weight: 3290
url: /es/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Especifica una conexión de datos externa

```csharp
public abstract class ExternalConnection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indica si la conexión se puede actualizar en segundo plano (asincrónicamente). verdadero si el uso preferido de la conexión es actualizar de forma asíncrona en segundo plano; falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Especifica la descripción de usuario para esta conexión |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Especifica el identificador único de esta conexión. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Obtiene el id de la conexión. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indica si se eliminó la conexión del libro de trabajo asociado. true si se ha eliminado la conexión ; de lo contrario, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True si la conexión no se ha actualizado por primera vez; en caso contrario, falso. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de regresar. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener abierta la conexión . Cuando es falso, la aplicación debe cerrar la conexión después de recuperar la información . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Especifica la ruta completa al archivo de conexión externa a partir del cual se creó esta conexión . Si falla una conexión durante un intento de actualizar los datos y reconnectionMethod=1, , la aplicación de hoja de cálculo volverá a intentarlo utilizando la información del archivo de conexión externo en lugar del objeto de conexión incrustado en el libro de trabajo. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indica si la aplicación de hoja de cálculo debe usar siempre y solo la información de conexión en el archivo de conexión externo indicado por el atributo odcFile cuando se actualiza la conexión. Si es falso, la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Obtiene[`ConnectionParameterCollection`](../connectionparametercollection) para una consulta ODBC o web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Obtiene la definición de la fórmula power query. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Especifica qué debe hacer la aplicación de hoja de cálculo cuando falla una conexión. El valor predeterminado es ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Especifica la cantidad de minutos entre actualizaciones automáticas de la conexión. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True si esta conexión debe actualizarse al abrir el archivo; de lo contrario, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Verdadero si los datos externos obtenidos a través de la conexión para completar una tabla deben guardarse con el libro de trabajo; en caso contrario, falso. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True si la contraseña se guardará como parte de la cadena de conexión; de lo contrario, Falso. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Se utiliza cuando el origen de datos externo está basado en archivos. Cuando falla una conexión a dicha fuente de datos , la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede ser expresado en URI o notación de ruta de archivo específica del sistema. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identificador para inicio de sesión único (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Obtiene o establece el tipo de origen de datos de la conexión externa. |

### Ver también

* espacio de nombres [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

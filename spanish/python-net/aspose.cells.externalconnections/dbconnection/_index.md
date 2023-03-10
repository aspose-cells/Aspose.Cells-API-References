---
title: DBConnection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection clase
Especifica todas las propiedades asociadas con una conexión de datos externa ODBC u OLE DB.



**Herencia:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)



El tipo DBConnection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [id](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/id) | Obtiene el id de la conexión.|
| [power_query_formula](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Obtiene la definición de la fórmula de consulta de potencia.|
| [type](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/type) | Obtiene o establece el tipo de origen de datos de la conexión externa.|
| [source_file](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Se utiliza cuando la fuente de datos externa está basada en archivos. Cuando una conexión a tales datos<br/> fuente falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Tal vez<br/> expresado en URI o notación de ruta de archivo específica del sistema.|
| [sso_id](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Identificador de inicio de sesión único (SSO) utilizado para la autenticación entre un intermediario<br/> servidor spreadsheetML y la fuente de datos externa.|
| [save_password](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/save_password) | True si la contraseña se guardará como parte de la cadena de conexión; de lo contrario, Falso.|
| [save_data](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/save_data) | True si se van a guardar los datos externos obtenidos a través de la conexión para completar una tabla<br/> con el libro de trabajo; en caso contrario, falso.|
| [refresh_on_load](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | True si esta conexión debe actualizarse al abrir el archivo; en caso contrario, falso.|
| [reconnection_method_type](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Especifica lo que debe hacer la aplicación de hoja de cálculo cuando falla una conexión.<br/>El valor predeterminado es ReConnectionMethodType.Required.|
| [reconnection_method](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Especifica lo que debe hacer la aplicación de hoja de cálculo cuando falla una conexión.<br/>El valor predeterminado es ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Indica si la aplicación de hoja de cálculo debe usar siempre y solo el<br/> información de conexión en el archivo de conexión externo indicado por el atributo odcFile<br/> cuando se actualiza la conexión. Si es falso, entonces la aplicación de hoja de cálculo<br/> debe seguir el procedimiento indicado por el atributo reconnectionMethod|
| [odc_file](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Especifica la ruta completa al archivo de conexión externa desde el que se realizó esta conexión.<br/> creado. Si una conexión falla durante un intento de actualizar los datos y reconnectionMethod=1,<br/> luego, la aplicación de hoja de cálculo volverá a intentarlo utilizando la información del archivo de conexión externa<br/> en lugar del objeto de conexión incrustado en el libro de trabajo.|
| [is_new](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/is_new) | True si la conexión no se ha actualizado por primera vez; en caso contrario, falso.<br/> Este estado puede ocurrir cuando el usuario guarda el archivo antes de que termine de regresar una consulta.|
| [name](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/name) | Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.|
| [keep_alive](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión<br/>abierto. Cuando es falso, la aplicación debe cerrar la conexión después de recuperar el<br/> información.|
| [refresh_internal](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Especifica la cantidad de minutos entre actualizaciones automáticas de la conexión.|
| [connection_id](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Especifica el identificador único de esta conexión.|
| [connection_description](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Especifica la descripción del usuario para esta conexión.|
| [is_deleted](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |Indica si se ha eliminado la conexión del libro de trabajo asociado. cierto si el<br/> la conexión ha sido eliminada; en caso contrario, falso.|
| [credentials_method_type](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.|
| [credentials](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.|
| [background_refresh](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Indica si la conexión se puede actualizar en segundo plano (asincrónicamente).<br/>true si el uso preferido de la conexión es actualizar de forma asíncrona en segundo plano;<br/> falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano.|
| [parameters](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/parameters) | Obtiene [ConnectionParameterCollection](/cells/es/python-net/aspose.cells.externalconnections/connectionparametercollection) para una consulta web o ODBC.|
| [connection_info](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | La cadena de información de conexión se utiliza para establecer contacto con una fuente de datos OLE DB u ODBC.|
| [command_type](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/command_type) | Especifica el tipo de comando OLE DB.<br/>1. La consulta especifica un nombre de cubo<br/>2. Consulta especifica una declaración SQL<br/>3. Consulta especifica un nombre de tabla<br/>4. La consulta especifica que se ha proporcionado información predeterminada y depende del proveedor cómo interpretarla.<br/> 5. La consulta es contra un proveedor de datos de lista basado en la web.|
| [command](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/command) | La cadena que contiene el comando de base de datos para pasar al proveedor de datos API que<br/> interactuar con la fuente externa para recuperar datos|
| [sever_command](/cells/es/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |Especifica una segunda cadena de texto de comando que se conserva cuando se basa en un servidor de tabla dinámica.<br/> los campos de la página están en uso.<br/> Para las conexiones ODBC, serverCommand suele ser una consulta más amplia que el comando (no<br/>La cláusula WHERE está presente en el primero). Basado en estos 2 comandos (Command y ServerCommand),<br/> la interfaz de usuario del parámetro se puede completar y las consultas parametrizadas se pueden construir|



###  Ver también
* módulo [aspose.cells.externalconnections](..)
* clase [ConnectionParameterCollection](/cells/es/python-net/aspose.cells.externalconnections/connectionparametercollection)
* clase [DBConnection](/cells/es/python-net/aspose.cells.externalconnections/dbconnection)
* clase [ExternalConnection](/cells/es/python-net/aspose.cells.externalconnections/externalconnection)

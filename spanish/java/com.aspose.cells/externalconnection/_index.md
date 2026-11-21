---
title: "ExternalConnection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica una conexión de datos externa"
type: docs
url: /es/java/com.aspose.cells/externalconnection/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExternalConnection
```

Especifica una conexión de datos externa
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indica si la conexión puede actualizarse en segundo plano (asíncronamente). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Obtiene el tipo de este objeto [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos. |
| [getCommandType()](#getCommandType--) | Especifica el tipo de comando OLE DB. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | Especifica la descripción del usuario para esta conexión. |
| [getConnectionFile()](#getConnectionFile--) | Obtiene el archivo de conexión. |
| [getConnectionId()](#getConnectionId--) | Especifica el identificador único de esta conexión. |
| [getConnectionString()](#getConnectionString--) | La cadena de información de conexión se utiliza para contactar con una fuente de datos OLE DB u ODBC. |
| [getCredentials()](#getCredentials--) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [getId()](#getId--) | Obtiene el id de la conexión. |
| [getKeepAlive()](#getKeepAlive--) | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. |
| [getName()](#getName--) | Especifica el nombre de la conexión. |
| [getOdcFile()](#getOdcFile--) | Especifica la ruta completa al archivo de conexión externo desde el cual se creó esta conexión. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externo indicado por el atributo odcFile cuando se actualiza la conexión. |
| [getParameters()](#getParameters--) | Obtiene [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) para una consulta ODBC o web. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Obtiene la definición de la fórmula Power Query. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión. |
| [getRefreshInternal()](#getRefreshInternal--) | Especifica el número de minutos entre actualizaciones automáticas de la conexión. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso. |
| [getSSOId()](#getSSOId--) | Identificador para Single Sign On (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. |
| [getSaveData()](#getSaveData--) | Verdadero si los datos externos obtenidos a través de la conexión para poblar una tabla deben guardarse con el libro de trabajo; de lo contrario, falso. |
| [getSavePassword()](#getSavePassword--) | Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso. |
| [getSecondCommand()](#getSecondCommand--) | Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. |
| [getSourceFile()](#getSourceFile--) | Se utiliza cuando la fuente de datos externa es basada en archivos. |
| [getSourceType()](#getSourceType--) | Obtiene el tipo de DataSource de la conexión externa. |
| [getType()](#getType--) | Obtiene el tipo de DataSource de la conexión externa. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Indica si la conexión del libro de trabajo asociada ha sido eliminada. |
| [isNew()](#isNew--) | Verdadero si la conexión no se ha actualizado por primera vez; de lo contrario, falso. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Indica si la conexión puede actualizarse en segundo plano (asíncronamente). |
| [setCommand(String value)](#setCommand-java.lang.String-) | La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos. |
| [setCommandType(int value)](#setCommandType-int-) | Especifica el tipo de comando OLE DB. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Especifica la descripción del usuario para esta conexión. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | La cadena de información de conexión se utiliza para contactar con una fuente de datos OLE DB u ODBC. |
| [setCredentials(int value)](#setCredentials-int-) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica si la conexión del libro de trabajo asociada ha sido eliminada. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. |
| [setName(String value)](#setName-java.lang.String-) | Especifica el nombre de la conexión. |
| [setNew(boolean value)](#setNew-boolean-) | Verdadero si la conexión no se ha actualizado por primera vez; de lo contrario, falso. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Especifica la ruta completa al archivo de conexión externo desde el cual se creó esta conexión. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externo indicado por el atributo odcFile cuando se actualiza la conexión. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Especifica el número de minutos entre actualizaciones automáticas de la conexión. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Identificador para Single Sign On (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Verdadero si los datos externos obtenidos a través de la conexión para poblar una tabla deben guardarse con el libro de trabajo; de lo contrario, falso. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Se utiliza cuando la fuente de datos externa es basada en archivos. |
| [setSourceType(int value)](#setSourceType-int-) | Establece el tipo de DataSource de la conexión externa. |
| [setType(int value)](#setType-int-) | Establece el tipo de DataSource de la conexión externa. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Indica si la conexión puede actualizarse en segundo plano (asíncronamente). verdadero si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClassType() {#getClassType--}
```
public abstract int getClassType()
```


Obtiene el tipo de este objeto [ExternalConnection](../../com.aspose.cells/externalconnection).

Ver [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta especifica que se ha proporcionado información predeterminada, y depende del proveedor cómo interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web.

Ver [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Especifica la descripción del usuario para esta conexión.

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Obtiene el archivo de conexión.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Especifica el identificador único de esta conexión.

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.Id. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


La cadena de información de conexión se utiliza para contactar con una fuente de datos OLE DB u ODBC.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.

Ver [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.CredentialsMethodType. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.

Ver [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Obtiene el id de la conexión.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. Cuando falso, la aplicación debe cerrar la conexión después de recuperar la información.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro de trabajo.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si falso, la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Obtiene [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) para una consulta ODBC o web.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Obtiene la definición de la fórmula Power Query.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

Ver [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.ReconnectionMethodType. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

Ver [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Especifica el número de minutos entre actualizaciones automáticas de la conexión.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identificador para Single Sign On (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Verdadero si los datos externos obtenidos a través de la conexión para poblar una tabla deben guardarse con el libro de trabajo; de lo contrario, falso.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE en la primera). Basándose en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Se utiliza cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación URI o ruta de archivo específica del sistema.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Obtiene el tipo de DataSource de la conexión externa.

Ver [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de DataSource de la conexión externa.

Ver [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad ExternalConnection.SourceType. Esta propiedad será eliminada 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundRefresh(boolean value) {#setBackgroundRefresh-boolean-}
```
public void setBackgroundRefresh(boolean value)
```


Indica si la conexión puede actualizarse en segundo plano (asíncronamente). verdadero si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; falso si el uso preferido de la conexión es actualizar sincrónicamente en primer plano.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta especifica que se ha proporcionado información predeterminada, y depende del proveedor cómo interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web.

Ver [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Especifica la descripción del usuario para esta conexión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


La cadena de información de conexión se utiliza para contactar con una fuente de datos OLE DB u ODBC.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.

Ver [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.CredentialsMethodType. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Especifica el método de autenticación que se utilizará al establecer (o restablecer) la conexión.

Ver [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indica si la conexión del libro de trabajo asociada ha sido eliminada. true si la conexión ha sido eliminada; de lo contrario, false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


Verdadero cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. Cuando falso, la aplicación debe cerrar la conexión después de recuperar la información.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Indica si la aplicación de hoja de cálculo debe siempre y únicamente usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si falso, la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

Ver [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.ReconnectionMethodType. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2017. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

Ver [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Especifica el número de minutos entre actualizaciones automáticas de la conexión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


Verdadero si esta conexión debe actualizarse al abrir el archivo; de lo contrario, falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Identificador para Single Sign On (SSO) utilizado para la autenticación entre un servidor intermedio spreadsheetML y la fuente de datos externa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Verdadero si los datos externos obtenidos a través de la conexión para poblar una tabla deben guardarse con el libro de trabajo; de lo contrario, falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


Verdadero si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, Falso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE en la primera). Basándose en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Se utiliza cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación URI o ruta de archivo específica del sistema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Establece el tipo de DataSource de la conexión externa.

Ver [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de DataSource de la conexión externa.

Ver [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad ExternalConnection.SourceType. Esta propiedad será eliminada 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


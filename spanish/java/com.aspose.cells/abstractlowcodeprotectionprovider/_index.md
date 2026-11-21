---
title: "AbstractLowCodeProtectionProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación para proporcionar configuraciones de protección"
type: docs
url: /es/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Implementación para proporcionar configuraciones de protección
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Obtiene la contraseña para abrir el archivo de hoja de cálculo. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Obtiene la contraseña para proteger el libro con el tipo de protección especificado. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Obtiene el tipo de protección para proteger el libro. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Obtiene la contraseña para proteger la hoja de cálculo especificada. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Obtiene el tipo de protección para proteger la hoja de cálculo especificada. |
| [getWritePassword()](#getWritePassword--) | Obtiene la contraseña para modificar el archivo de hoja de cálculo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Obtiene la contraseña para abrir el archivo de hoja de cálculo.

**Returns:**
java.lang.String - Contraseña para abrir el archivo de hoja de cálculo. Vacío significa que no hay protección al abrir el archivo.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Obtiene la contraseña para proteger el libro con el tipo de protección especificado.

**Returns:**
java.lang.String - Contraseña para proteger el libro.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Obtiene el tipo de protección para proteger el libro.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección para proteger el libro. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) significa que no hay protección para el libro.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Obtiene la contraseña para proteger la hoja de cálculo especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Contraseña para proteger la hoja de cálculo especificada.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Obtiene el tipo de protección para proteger la hoja de cálculo especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección para proteger la hoja de cálculo especificada. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) significa que no hay protección para la hoja de cálculo.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Obtiene la contraseña para modificar el archivo de hoja de cálculo.

**Returns:**
java.lang.String - Contraseña para modificar el archivo de hoja de cálculo. Vacío significa que no hay protección para modificar el archivo.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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


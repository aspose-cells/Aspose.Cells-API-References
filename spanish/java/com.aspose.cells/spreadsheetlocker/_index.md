---
title: "SpreadsheetLocker"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "API de bajo código para bloquear el archivo de hoja de cálculo."
type: docs
url: /es/java/com.aspose.cells/spreadsheetlocker/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetLocker
```

API de bajo código para bloquear el archivo de hoja de cálculo.

**Example**

```
         SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
| [process(String templateFile, String resultFile, String openPassword, String writePassword)](#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Bloquea el archivo de hoja de cálculo con la configuración especificada. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)
```


Bloquea el archivo de hoja de cálculo con la configuración especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opciones para entrada y carga |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opciones para salida y guardado |
| provider | [AbstractLowCodeProtectionProvider](../../com.aspose.cells/abstractlowcodeprotectionprovider) | Implementación para proporcionar configuraciones de protección |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)
```


Bloquea el archivo de hoja de cálculo con la configuración especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opciones para entrada y carga |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opciones para salida y guardado |
| openPassword | java.lang.String | Contraseña para el cifrado de archivos |
| writePassword | java.lang.String | Contraseña para la protección de la modificación de la hoja de cálculo |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)
```


Bloquea el archivo de hoja de cálculo con la configuración especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opciones para entrada y carga |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opciones para salida y guardado |
| openPassword | java.lang.String | Contraseña para el cifrado de archivos |
| writePassword | java.lang.String | Contraseña para la protección de la modificación de la hoja de cálculo |
| workbookPassword | java.lang.String | Contraseña para la protección del libro de trabajo |
| workbookType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección para proteger el libro de trabajo |

### process(String templateFile, String resultFile, String openPassword, String writePassword) {#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile, String openPassword, String writePassword)
```


Bloquea el archivo de hoja de cálculo con la configuración especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | java.lang.String | El archivo de plantilla a bloquear |
| resultFile | java.lang.String | El archivo resultante |
| openPassword | java.lang.String | Contraseña para el cifrado de archivos |
| writePassword | java.lang.String | Contraseña para la protección de la modificación de la hoja de cálculo |

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


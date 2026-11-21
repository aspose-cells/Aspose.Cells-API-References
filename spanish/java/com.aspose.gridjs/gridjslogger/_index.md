---
title: "GridJsLogger"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Proporciona un sistema de registro ligero para el servidor GridJs."
type: docs
url: /es/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Proporciona un sistema de registro ligero para el servidor GridJs. Soporta salida a consola y archivo con niveles de registro configurables. El nivel predeterminado es Ninguno. En compilación DEBUG, el nivel predeterminado es Depuración (muestra todos los mensajes). Soporta la rotación de archivos de registro por día/semana/mes.
## Métodos

| Método | Descripción |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Cierra el escritor del archivo de registro y desactiva la salida a archivo. |
| [debug(String message)](#debug-java.lang.String-) | Registra un mensaje de nivel depuración. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Registra un mensaje de nivel error. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Obtiene si se deben enviar los mensajes de registro a la consola. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Obtiene si se deben enviar los mensajes de registro a un archivo. |
| [getLevel()](#getLevel--) | Obtiene el nivel mínimo de registro. |
| [getLogFilePath()](#getLogFilePath--) | Obtiene la ruta actual del archivo de registro, o nulo si no está establecida. |
| [getMaxFileSize()](#getMaxFileSize--) | Obtiene el tamaño máximo (en bytes) de un archivo de registro antes de rotar. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Registra un mensaje de nivel información. |
| [log(int level, String message)](#log-int-java.lang.String-) | Registra un mensaje en el nivel especificado. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Establece si se deben enviar los mensajes de registro a la consola. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Establece si se deben enviar los mensajes de registro a un archivo. |
| [setLevel(int value)](#setLevel-int-) | Establece el nivel mínimo de registro. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Establece el directorio de registro con estrategia de archivo rotativo diario y habilita la salida a archivo. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Establece el directorio de registro con estrategia de archivo rotativo y habilita la salida a archivo. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Establece el directorio de registro con estrategia de archivo rotativo y habilita la salida a archivo. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Establece el tamaño máximo (en bytes) de un archivo de registro antes de rotar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Registra un mensaje de nivel de advertencia. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Cierra el escritor del archivo de registro y desactiva la salida a archivo.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Registra un mensaje de nivel depuración.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mensaje | java.lang.String |  |

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
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Registra un mensaje de nivel error.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mensaje | java.lang.String |  |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableConsoleOutput() {#getEnableConsoleOutput--}
```
public static boolean getEnableConsoleOutput()
```


Obtiene si se deben enviar los mensajes de registro a la consola. El valor predeterminado es false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Obtiene si se deben enviar los mensajes de registro a un archivo. El valor predeterminado es false. Debe llamar a [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\\#setLogFile-String-) o [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\\#setLogDirectory-String-) antes de habilitar.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Obtiene el nivel mínimo de registro. Los mensajes por debajo de este nivel serán ignorados. El valor predeterminado es None.

Ver [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Obtiene la ruta actual del archivo de registro, o nulo si no está establecida.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Obtiene el tamaño máximo (en bytes) de un archivo de registro antes de rotar. Solo es efectivo cuando la rotación está habilitada. 0 significa sin límite de tamaño. El valor predeterminado es 0.

**Returns:**
long
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### info(String message) {#info-java.lang.String-}
```
public static void info(String message)
```


Registra un mensaje de nivel información.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mensaje | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Registra un mensaje en el nivel especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). El nivel de registro. |
| mensaje | java.lang.String | El mensaje a registrar. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setEnableConsoleOutput(boolean value) {#setEnableConsoleOutput-boolean-}
```
public static void setEnableConsoleOutput(boolean value)
```


Establece si se deben enviar los mensajes de registro a la consola. El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Establece si se deben enviar los mensajes de registro a un archivo. El valor predeterminado es false. Debe llamar a [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\\#setLogFile-String-) o [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\\#setLogDirectory-String-) antes de habilitar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Establece el nivel mínimo de registro. Los mensajes por debajo de este nivel serán ignorados. El valor predeterminado es None.

Ver [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Establece el directorio de registro con estrategia de archivo rotativo diario y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs\\_\\{period\\}.log

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.lang.String | El directorio donde se almacenan los archivos de registro. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Establece el directorio de registro con estrategia de archivo rotativo y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs\\_\\{period\\}.log

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.lang.String | El directorio donde se almacenan los archivos de registro. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La estrategia de rotación (Diaria/Semanal/Mensual). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Establece el directorio de registro con estrategia de archivo rotativo y habilita la salida a archivo. Los archivos de registro se nombrarán como: \\{prefix\\}\\_\\{period\\}.log Ejemplos: gridjs\\_2026-07-27.log (Diario), gridjs\\_2026-W30.log (Semanal), gridjs\\_2026-07.log (Mensual)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.lang.String | El directorio donde se almacenan los archivos de registro. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La estrategia de rotación (Diaria/Semanal/Mensual). |
| filePrefix | java.lang.String | El prefijo del nombre de archivo. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación). Añade al archivo existente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta completa al archivo de registro. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta completa al archivo de registro. |
| añadir | boolean | Indica si se debe añadir al archivo existente. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Establece el tamaño máximo (en bytes) de un archivo de registro único antes de rotar. Solo es efectivo cuando la rotación está habilitada. 0 significa sin límite de tamaño. El valor predeterminado es 0.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | long |  |

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

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Registra un mensaje de nivel de advertencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mensaje | java.lang.String |  |


---
title: "GridJsLogger"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillhandahåller ett lättviktigt loggningssystem för GridJs-servern."
type: docs
url: /sv/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Tillhandahåller ett lättviktigt loggningssystem för GridJs‑servern. Stöder konsol‑ och filutmatning med konfigurerbara loggnivåer. Standardnivån är None. I DEBUG‑byggnad är standardnivån Debug (utskriver alla meddelanden). Stöder rullning av loggfil per dag/vecka/månad.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Stänger loggfilsskrivaren och inaktiverar filutmatning. |
| [debug(String message)](#debug-java.lang.String-) | Loggar ett meddelande på debug‑nivå. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Loggar ett meddelande på fel‑nivå. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Hämtar om loggmeddelanden ska skrivas ut till konsolen. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Hämtar om loggmeddelanden ska skrivas ut till en fil. |
| [getLevel()](#getLevel--) | Hämtar den minsta loggnivån. |
| [getLogFilePath()](#getLogFilePath--) | Hämtar den aktuella sökvägen till loggfilen, eller null om den inte är angiven. |
| [getMaxFileSize()](#getMaxFileSize--) | Hämtar den maximala storleken (i byte) för en enskild loggfil innan den rullas. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Loggar ett meddelande på info-nivå. |
| [log(int level, String message)](#log-int-java.lang.String-) | Loggar ett meddelande på den angivna nivån. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Ställer in om loggmeddelanden ska skrivas ut till konsolen. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Ställer in om loggmeddelanden ska skrivas till en fil. |
| [setLevel(int value)](#setLevel-int-) | Ställer in den minsta loggnivån. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Ställer in loggmappen med daglig rullningsstrategi och aktiverar filutmatning. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Ställer in loggmappen med rullningsstrategi och aktiverar filutmatning. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Ställer in loggmappen med rullningsstrategi och aktiverar filutmatning. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Ställer in sökvägen till loggfilen och aktiverar filutmatning (enkelfilsläge, ingen rullning). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Ställer in sökvägen till loggfilen och aktiverar filutmatning (enkelfilsläge, ingen rullning). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Ställer in den maximala storleken (i byte) för en enskild loggfil innan rullning. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Loggar ett varningsmeddelande. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Stänger loggfilsskrivaren och inaktiverar filutmatning.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Loggar ett meddelande på debug‑nivå.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Loggar ett meddelande på fel‑nivå.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |

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


Hämtar om loggmeddelanden ska skrivas ut till konsolen. Standard är falskt.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Hämtar om loggmeddelanden ska skrivas till en fil. Standard är falskt. Måste anropa [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) eller [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) innan aktivering.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Hämtar den minsta loggnivån. Meddelanden under denna nivå ignoreras. Standard är Ingen.

Se [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Hämtar den aktuella sökvägen till loggfilen, eller null om den inte är angiven.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Hämtar den maximala storleken (i byte) för en enskild loggfil innan rullning. Gäller endast när rullning är aktiverad. 0 betyder ingen storleksgräns. Standard är 0.

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


Loggar ett meddelande på info-nivå.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Loggar ett meddelande på den angivna nivån.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Loggnivån. |
| meddelande | java.lang.String | Meddelandet att logga. |

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


Ställer in om loggmeddelanden ska skrivas ut till konsolen. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Ställer in om loggmeddelanden ska skrivas till en fil. Standard är falskt. Måste anropa [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) eller [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) innan aktivering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Ställer in den minsta loggnivån. Meddelanden under denna nivå ignoreras. Standard är Ingen.

Se [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Ställer in loggmappen med daglig rullningsstrategi och aktiverar filutmatning. Loggfiler kommer att namnges som: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | java.lang.String | Katalogen för att lagra loggfiler. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Ställer in loggkatalogen med rullande filstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | java.lang.String | Katalogen för att lagra loggfiler. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Den rullningsstrategi (Daily/Weekly/Monthly). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Ställer in loggkatalogen med rullande filstrategi och aktiverar filutmatning. Loggfilerna kommer att namnges som: \{prefix\}\_\{period\}.log Exempel: gridjs\_2026-07-27.log (Daily), gridjs\_2026-W30.log (Weekly), gridjs\_2026-07.log (Monthly)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| katalog | java.lang.String | Katalogen för att lagra loggfiler. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Den rullningsstrategi (Daily/Weekly/Monthly). |
| filePrefix | java.lang.String | Filnamnsprefixet. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Ställer in sökvägen för loggfilen och aktiverar filutmatning (enkel filläge, ingen rullning). Lägger till i befintlig fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Den fullständiga sökvägen till loggfilen. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Ställer in sökvägen till loggfilen och aktiverar filutmatning (enkelfilsläge, ingen rullning).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Den fullständiga sökvägen till loggfilen. |
| lägg till | boolean | Om den ska läggas till i befintlig fil. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Ställer in maximal storlek (i byte) för en enskild loggfil innan rullning. Endast effektiv när rullning är aktiverad. 0 betyder ingen storleksgräns. Standard är 0.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | long |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Loggar ett varningsmeddelande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |


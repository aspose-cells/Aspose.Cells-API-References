---
title: "GridJsLogger"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Bietet ein leichtgewichtiges Protokollierungssystem für den GridJs-Server"
type: docs
url: /de/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Bietet ein leichtgewichtiges Protokollierungssystem für den GridJs‑Server. Unterstützt Konsolen‑ und Dateiausgabe mit konfigurierbaren Protokollstufen. Standardstufe ist None. Im DEBUG‑Build ist die Standardstufe Debug (gibt alle Meldungen aus). Unterstützt das Rollen von Protokolldateien nach Tag/Woche/Monat.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Schließt den Protokolldateischreiber und deaktiviert die Dateiausgabe. |
| [debug(String message)](#debug-java.lang.String-) | Protokolliert eine Meldung auf Debug‑Stufe. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Protokolliert eine Meldung auf Fehler‑Stufe. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Ermittelt, ob Protokollmeldungen in die Konsole ausgegeben werden. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Ermittelt, ob Protokollmeldungen in eine Datei ausgegeben werden. |
| [getLevel()](#getLevel--) | Ermittelt die minimale Protokollstufe. |
| [getLogFilePath()](#getLogFilePath--) | Ermittelt den aktuellen Protokolldateipfad oder null, wenn nicht festgelegt. |
| [getMaxFileSize()](#getMaxFileSize--) | Ermittelt die maximale Größe (in Bytes) einer einzelnen Protokolldatei vor dem Rollen. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Protokolliert eine Meldung auf Info‑Stufe. |
| [log(int level, String message)](#log-int-java.lang.String-) | Protokolliert eine Meldung auf der angegebenen Stufe. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Legt fest, ob Protokollmeldungen in die Konsole ausgegeben werden. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Legt fest, ob Protokollmeldungen in eine Datei ausgegeben werden. |
| [setLevel(int value)](#setLevel-int-) | Setzt die minimale Protokollstufe. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Setzt das Protokollverzeichnis mit täglicher Rollen‑Dateistrategie und aktiviert die Dateiausgabe. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Setzt das Protokollverzeichnis mit Rollen‑Dateistrategie und aktiviert die Dateiausgabe. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Setzt das Protokollverzeichnis mit Rollen‑Dateistrategie und aktiviert die Dateiausgabe. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Setzt den Protokolldateipfad und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Setzt den Protokolldateipfad und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Setzt die maximale Größe (in Bytes) einer einzelnen Protokolldatei vor dem Rollen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Protokolliert eine Meldung auf Warn‑Stufe. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Schließt den Protokolldateischreiber und deaktiviert die Dateiausgabe.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Protokolliert eine Meldung auf Debug‑Stufe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Nachricht | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Protokolliert eine Meldung auf Fehler‑Stufe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Nachricht | java.lang.String |  |

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


Ermittelt, ob Protokollmeldungen in die Konsole ausgegeben werden. Standard ist false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Ermittelt, ob Protokollmeldungen in eine Datei ausgegeben werden. Standard ist false. Vor dem Aktivieren muss [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) oder [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) aufgerufen werden.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Ermittelt die minimale Protokollstufe. Meldungen unterhalb dieser Stufe werden ignoriert. Standard ist None.

Siehe [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Ermittelt den aktuellen Protokolldateipfad oder null, wenn nicht festgelegt.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Ermittelt die maximale Größe (in Bytes) einer einzelnen Protokolldatei vor dem Rollen. Nur wirksam, wenn Rollen aktiviert ist. 0 bedeutet keine Größenbeschränkung. Standard ist 0.

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


Protokolliert eine Meldung auf Info‑Stufe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Nachricht | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Protokolliert eine Meldung auf der angegebenen Stufe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Der Protokollierungsgrad. |
| Nachricht | java.lang.String | Die zu protokollierende Nachricht. |

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


Legt fest, ob Protokollnachrichten in die Konsole ausgegeben werden. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Legt fest, ob Protokollnachrichten in eine Datei ausgegeben werden. Standard ist false. Vor dem Aktivieren muss [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) oder [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) aufgerufen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Legt den minimalen Protokollierungsgrad fest. Nachrichten unter diesem Grad werden ignoriert. Standard ist Keine.

Siehe [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Legt das Protokollverzeichnis mit täglicher Rollierungsstrategie fest und aktiviert die Dateiausgabe. Protokolldateien werden benannt als: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.lang.String | Das Verzeichnis zum Speichern von Protokolldateien. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Legt das Protokollverzeichnis mit Rollierungsstrategie fest und aktiviert die Dateiausgabe. Protokolldateien werden benannt als: gridjs\_\{period\}.log

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.lang.String | Das Verzeichnis zum Speichern von Protokolldateien. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Die Rollierungsstrategie (Täglich/Wöchentlich/Monatlich). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Legt das Protokollverzeichnis mit Rollierungsstrategie fest und aktiviert die Dateiausgabe. Protokolldateien werden benannt als: \{prefix\}\_\{period\}.log Beispiele: gridjs\_2026-07-27.log (Täglich), gridjs\_2026-W30.log (Wöchentlich), gridjs\_2026-07.log (Monatlich)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.lang.String | Das Verzeichnis zum Speichern von Protokolldateien. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). Die Rollierungsstrategie (Täglich/Wöchentlich/Monatlich). |
| filePrefix | java.lang.String | Das Dateinamenpräfix. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Legt den Pfad der Protokolldatei fest und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen). Hängt an die bestehende Datei an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der vollständige Pfad zur Protokolldatei. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Setzt den Protokolldateipfad und aktiviert die Dateiausgabe (Einzeldateimodus, kein Rollen).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der vollständige Pfad zur Protokolldatei. |
| anhängen | boolean | Ob an die bestehende Datei angehängt werden soll. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Legt die maximale Größe (in Bytes) einer einzelnen Protokolldatei vor dem Rollen fest. Nur wirksam, wenn Rollen aktiviert ist. 0 bedeutet keine Größenbeschränkung. Standard ist 0.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | long |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Protokolliert eine Meldung auf Warn‑Stufe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Nachricht | java.lang.String |  |


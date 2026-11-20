---
title: "GridJsLogger"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce un sistema di logging leggero per il server GridJs."
type: docs
url: /it/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Fornisce un sistema di logging leggero per il server GridJs. Supporta l'output su console e file con livelli di log configurabili. Il livello predefinito è None. In build DEBUG, il livello predefinito è Debug (emette tutti i messaggi). Supporta il rollover dei file di log per giorno/settimana/mese.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Chiude lo scrittore del file di log e disabilita l'output su file. |
| [debug(String message)](#debug-java.lang.String-) | Registra un messaggio di livello debug. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Registra un messaggio di livello errore. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Restituisce se inviare i messaggi di log alla console. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Restituisce se inviare i messaggi di log a un file. |
| [getLevel()](#getLevel--) | Restituisce il livello di log minimo. |
| [getLogFilePath()](#getLogFilePath--) | Restituisce il percorso corrente del file di log, o null se non impostato. |
| [getMaxFileSize()](#getMaxFileSize--) | Restituisce la dimensione massima (in byte) per un singolo file di log prima del rollover. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Registra un messaggio di livello info. |
| [log(int level, String message)](#log-int-java.lang.String-) | Registra un messaggio al livello specificato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Imposta se inviare i messaggi di log alla console. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Imposta se inviare i messaggi di log a un file. |
| [setLevel(int value)](#setLevel-int-) | Imposta il livello minimo di log. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Imposta la directory dei log con strategia di rotazione giornaliera dei file e abilita l'output su file. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Imposta la directory dei log con strategia di rotazione dei file e abilita l'output su file. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Imposta la directory dei log con strategia di rotazione dei file e abilita l'output su file. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Imposta il percorso del file di log e abilita l'output su file (modalità file singolo, senza rotazione). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Imposta il percorso del file di log e abilita l'output su file (modalità file singolo, senza rotazione). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Imposta la dimensione massima (in byte) per un singolo file di log prima della rotazione. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Registra un messaggio di livello avviso. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Chiude lo scrittore del file di log e disabilita l'output su file.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Registra un messaggio di livello debug.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Registra un messaggio di livello errore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |

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


Restituisce se inviare i messaggi di log alla console. Il valore predefinito è false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Restituisce se inviare i messaggi di log a un file. Il valore predefinito è false. È necessario chiamare [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) o [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) prima di abilitare.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Restituisce il livello minimo di log. I messaggi al di sotto di questo livello saranno ignorati. Il valore predefinito è Nessuno.

Vedi [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Restituisce il percorso corrente del file di log, o null se non impostato.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Restituisce la dimensione massima (in byte) per un singolo file di log prima della rotazione. È efficace solo quando la rotazione è abilitata. 0 significa nessun limite di dimensione. Il valore predefinito è 0.

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


Registra un messaggio di livello info.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Registra un messaggio al livello specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Il livello di log. |
| messaggio | java.lang.String | Il messaggio da registrare. |

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


Imposta se inviare i messaggi di log alla console. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Imposta se inviare i messaggi di log a un file. Il valore predefinito è false. È necessario chiamare [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) o [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) prima di abilitare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Imposta il livello minimo di log. I messaggi al di sotto di questo livello saranno ignorati. Il valore predefinito è Nessuno.

Vedi [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Imposta la directory dei log con strategia di rotazione giornaliera dei file e abilita l'output su file. I file di log saranno nominati così: gridjs\_\{period\}.log

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.lang.String | La directory in cui memorizzare i file di log. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Imposta la directory dei log con strategia di rotazione dei file e abilita l'output su file. I file di log saranno nominati così: gridjs\_\{period\}.log

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.lang.String | La directory in cui memorizzare i file di log. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La strategia di rotazione (Giornaliera/Settimanale/Mensile). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Imposta la directory dei log con strategia di rotazione dei file e abilita l'output su file. I file di log saranno nominati così: \{prefix\}\_\{period\}.log Esempi: gridjs\_2026-07-27.log (Giornaliero), gridjs\_2026-W30.log (Settimanale), gridjs\_2026-07.log (Mensile)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.lang.String | La directory in cui memorizzare i file di log. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La strategia di rotazione (Giornaliera/Settimanale/Mensile). |
| filePrefix | java.lang.String | Il prefisso del nome file. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Imposta il percorso del file di log e abilita l'output su file (modalità singolo file, senza rotazione). Aggiunge al file esistente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso completo del file di log. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Imposta il percorso del file di log e abilita l'output su file (modalità file singolo, senza rotazione).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso completo del file di log. |
| aggiungi | boolean | Indica se aggiungere al file esistente. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Imposta la dimensione massima (in byte) per un singolo file di log prima della rotazione. Valido solo quando la rotazione è abilitata. 0 indica nessun limite di dimensione. Il valore predefinito è 0.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | long |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Registra un messaggio di livello avviso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |


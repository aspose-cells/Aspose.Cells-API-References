---
title: "AbstractLowCodeProtectionProvider"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Implementazione per fornire impostazioni di protezione"
type: docs
url: /it/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Implementazione per fornire impostazioni di protezione
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Ottiene la password per aprire il file di foglio di calcolo. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Ottiene la password per proteggere la cartella di lavoro con il tipo di protezione specificato. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Ottiene il tipo di protezione per proteggere la cartella di lavoro. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Ottiene la password per proteggere il foglio di lavoro specificato. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Ottiene il tipo di protezione per proteggere il foglio di lavoro specificato. |
| [getWritePassword()](#getWritePassword--) | Ottiene la password per modificare il file di foglio di calcolo. |
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
| Parametro | Tipo | Descrizione |
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


Ottiene la password per aprire il file di foglio di calcolo.

**Returns:**
java.lang.String - Password per aprire il file di foglio di calcolo. Vuoto significa nessuna protezione per l'apertura del file.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Ottiene la password per proteggere la cartella di lavoro con il tipo di protezione specificato.

**Returns:**
java.lang.String - Password per proteggere la cartella di lavoro.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Ottiene il tipo di protezione per proteggere la cartella di lavoro.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Tipo di protezione per proteggere la cartella di lavoro. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) significa nessuna protezione per la cartella di lavoro.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Ottiene la password per proteggere il foglio di lavoro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Password per proteggere il foglio di lavoro specificato.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Ottiene il tipo di protezione per proteggere il foglio di lavoro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Tipo di protezione per proteggere il foglio di lavoro specificato. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) indica nessuna protezione per il foglio di lavoro.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Ottiene la password per modificare il file di foglio di calcolo.

**Returns:**
java.lang.String - Password per modificare il file del foglio di calcolo. Vuoto indica nessuna protezione per la modifica del file.
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


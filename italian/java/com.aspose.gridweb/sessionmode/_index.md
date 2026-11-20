---
title: "SessionMode"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la modalità di sessione della griglia."
type: docs
url: /it/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Rappresenta la modalità di sessione della griglia.
## Campi

| Campo | Descrizione |
| --- | --- |
| [CUSTOM](#CUSTOM) | Utilizza l'evento LoadCustomData per caricare manualmente i dati del foglio della griglia. |
| [FILE](#FILE) | Utilizza il file di sistema per memorizzare/ripristinare automaticamente i dati del foglio della griglia, l'utente deve impostare SessionStorePath per specificare la directory dei file. |
| [SESSION](#SESSION) | Utilizza la sessione di sistema per memorizzare/ripristinare automaticamente i dati del foglio della griglia. |
| [VIEW_STATE](#VIEW-STATE) | Utilizza lo viewstate della pagina per memorizzare/ripristinare automaticamente i dati del foglio della griglia. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Utilizza l'evento LoadCustomData per caricare manualmente i dati del foglio della griglia. E utilizza l'evento SheetDataUpdated per salvare i dati del foglio della griglia.

### FILE {#FILE}
```
public static final int FILE
```


Utilizza il file di sistema per memorizzare/ripristinare automaticamente i dati del foglio della griglia, l'utente deve impostare SessionStorePath per specificare la directory dei file.

### SESSION {#SESSION}
```
public static final int SESSION
```


Utilizza la sessione di sistema per memorizzare/ripristinare automaticamente i dati del foglio della griglia.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Utilizza lo viewstate della pagina per memorizzare/ripristinare automaticamente i dati del foglio della griglia.

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


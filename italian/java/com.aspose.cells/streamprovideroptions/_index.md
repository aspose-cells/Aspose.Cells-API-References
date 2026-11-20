---
title: "StreamProviderOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di stream."
type: docs
url: /it/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Rappresenta le opzioni di stream.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Inizializza una nuova istanza della classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Inizializza una nuova istanza della classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Il percorso personalizzato dell'utente (URL) salvato nel file HTML generato per la risorsa referenziata. |
| [getDefaultPath()](#getDefaultPath--) | Il percorso predefinito (URL) salvato nel file HTML generato per la risorsa referenziata. |
| [getInputStream()](#getInputStream--) | Ottiene lo stream di input per recuperare i dati. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Ottiene il tipo di risorsa di caricamento. |
| [getStream()](#getStream--) | Ottiene lo stream di output per scrivere i dati salvati. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Il percorso personalizzato dell'utente (URL) salvato nel file HTML generato per la risorsa referenziata. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Imposta lo stream di input per recuperare i dati. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Imposta il tipo di risorsa di caricamento. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Imposta lo stream di output per scrivere i dati salvati. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Inizializza una nuova istanza della classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Il tipo per caricare la risorsa collegata. |
| defaultPath | java.lang.String | Il percorso predefinito. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Inizializza una nuova istanza della classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


Il percorso personalizzato dell'utente (URL) salvato nel file HTML generato per la risorsa referenziata. Se non definito dall'utente, verrà utilizzato DefaultPath. Ad esempio, i dati del foglio saranno salvati dall'utente in d:/sheet001.htm, l'URL usato nel file HTML principale dovrebbe essere "d:/sheet001.htm" o un altro percorso relativo valido che possa essere accessibile dal file HTML principale.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Il percorso predefinito (URL) salvato nel file HTML generato per la risorsa referenziata. Ad esempio, i dati del foglio salvati in xxx\_files/sheet001.htm, l'URL usato nel file HTML principale dovrebbe essere del tipo "src=\"xxx\_files/sheet001.htm\""

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Ottiene lo stream di input per recuperare i dati.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Ottiene il tipo di risorsa di caricamento.

Vedi [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Ottiene lo stream di output per scrivere i dati salvati.

**Returns:**
java.io.OutputStream
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




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


Il percorso personalizzato dell'utente (URL) salvato nel file HTML generato per la risorsa referenziata. Se non definito dall'utente, verrà utilizzato DefaultPath. Ad esempio, i dati del foglio saranno salvati dall'utente in d:/sheet001.htm, l'URL usato nel file HTML principale dovrebbe essere "d:/sheet001.htm" o un altro percorso relativo valido che possa essere accessibile dal file HTML principale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Imposta lo stream di input per recuperare i dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Imposta il tipo di risorsa di caricamento.

Vedi [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Imposta lo stream di output per scrivere i dati salvati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.io.OutputStream |  |

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


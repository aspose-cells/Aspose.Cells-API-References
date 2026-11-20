---
title: "StreamProviderOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Stream‑Optionen dar."
type: docs
url: /de/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Stellt die Stream‑Optionen dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Initialisiert eine neue Instanz der Klasse [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Der benutzerdefinierte Pfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. |
| [getDefaultPath()](#getDefaultPath--) | Der Standardpfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. |
| [getInputStream()](#getInputStream--) | Liefert den Eingabestream zum Abrufen von Daten. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Liefert den Typ der zu ladenden Ressource. |
| [getStream()](#getStream--) | Liefert den Ausgabestream zum Schreiben der gespeicherten Daten. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Der benutzerdefinierte Pfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Setzt den Eingabestream zum Abrufen von Daten. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Setzt den Typ der zu ladenden Ressource. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Setzt den Ausgabestream zum Schreiben der gespeicherten Daten. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Initialisiert eine neue Instanz der Klasse [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Der Typ zum Laden der verknüpften Ressource. |
| defaultPath | java.lang.String | Der Standardpfad. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Initialisiert eine neue Instanz der Klasse [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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


Der benutzerdefinierte Pfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. Wenn er vom Benutzer nicht definiert wird, wird DefaultPath verwendet. Zum Beispiel wird das Blattdaten vom Benutzer nach d:/sheet001.htm gespeichert; die in der Haupt-HTML-Datei verwendete URL sollte "d:/sheet001.htm" oder ein anderer gültiger relativer Pfad sein, der von der Haupt-HTML-Datei aus erreichbar ist.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Der Standardpfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. Zum Beispiel werden die Blattdaten in xxx\\_files/sheet001.htm gespeichert; die in der Haupt-HTML-Datei verwendete URL sollte etwa "src=\"xxx\\_files/sheet001.htm\"" lauten.

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Liefert den Eingabestream zum Abrufen von Daten.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Liefert den Typ der zu ladenden Ressource.

Siehe [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Liefert den Ausgabestream zum Schreiben der gespeicherten Daten.

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


Der benutzerdefinierte Pfad (URL) wird in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert. Wenn er vom Benutzer nicht definiert wird, wird DefaultPath verwendet. Zum Beispiel wird das Blattdaten vom Benutzer nach d:/sheet001.htm gespeichert; die in der Haupt-HTML-Datei verwendete URL sollte "d:/sheet001.htm" oder ein anderer gültiger relativer Pfad sein, der von der Haupt-HTML-Datei aus erreichbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Setzt den Eingabestream zum Abrufen von Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Setzt den Typ der zu ladenden Ressource.

Siehe [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Setzt den Ausgabestream zum Schreiben der gespeicherten Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.io.OutputStream |  |

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


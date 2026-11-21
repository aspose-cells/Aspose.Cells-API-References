---
title: "StreamProviderOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar strömalternativen."
type: docs
url: /sv/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Representerar strömalternativen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Initierar en ny instans av klassen [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Initierar en ny instans av klassen [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Den användaranpassade sökvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. |
| [getDefaultPath()](#getDefaultPath--) | Den standardvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. |
| [getInputStream()](#getInputStream--) | Hämtar inmatningsströmmen för att få data. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Hämtar typen av laddningsresurs. |
| [getStream()](#getStream--) | Hämtar utmatningsströmmen för att skriva sparad data. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Den användaranpassade sökvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Ställer in inmatningsströmmen för att få data. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Ställer in typen av laddningsresurs. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Ställer in utmatningsströmmen för att skriva sparad data. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Initierar en ny instans av klassen [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Typen för att ladda den länkade resursen. |
| defaultPath | java.lang.String | Standardvägen. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Initierar en ny instans av klassen [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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


Den användardefinierade sökvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. Om den inte definieras av användaren används DefaultPath. Till exempel kommer bladdata att sparas av användaren till d:/sheet001.htm, URL:en som används i huvud‑HTML‑filen bör vara "d:/sheet001.htm" eller någon annan giltig relativ sökväg som kan nås av huvud‑HTML‑filen.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Standardvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. Till exempel, bladdata sparad i xxx\\_files/sheet001.htm, URL:en som används i huvud‑HTML‑filen bör vara som "src=\"xxx\\_files/sheet001.htm\""

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Hämtar inmatningsströmmen för att få data.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Hämtar typen av laddningsresurs.

Se [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Hämtar utmatningsströmmen för att skriva sparad data.

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


Den användardefinierade sökvägen (URL) som sparas i den genererade HTML-filen för den refererade källan. Om den inte definieras av användaren används DefaultPath. Till exempel kommer bladdata att sparas av användaren till d:/sheet001.htm, URL:en som används i huvud‑HTML‑filen bör vara "d:/sheet001.htm" eller någon annan giltig relativ sökväg som kan nås av huvud‑HTML‑filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Ställer in inmatningsströmmen för att få data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Ställer in typen av laddningsresurs.

Se [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Ställer in utmatningsströmmen för att skriva sparad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.io.OutputStream |  |

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


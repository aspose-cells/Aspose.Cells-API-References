---
title: "StreamProviderOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options du flux."
type: docs
url: /fr/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Représente les options du flux.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Initialise une nouvelle instance de la classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Initialise une nouvelle instance de la classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | Le chemin personnalisé de l'utilisateur (URL) enregistré dans le fichier HTML généré pour la source référencée. |
| [getDefaultPath()](#getDefaultPath--) | Le chemin par défaut (URL) enregistré dans le fichier HTML généré pour la source référencée. |
| [getInputStream()](#getInputStream--) | Obtient le flux d'entrée pour récupérer les données. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Obtient le type de ressource de chargement. |
| [getStream()](#getStream--) | Obtient le flux de sortie pour écrire les données enregistrées. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | Le chemin personnalisé de l'utilisateur (URL) enregistré dans le fichier HTML généré pour la source référencée. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Définit le flux d'entrée pour récupérer les données. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Définit le type de ressource de chargement. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Définit le flux de sortie pour écrire les données enregistrées. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Initialise une nouvelle instance de la classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). Le type pour charger la ressource liée. |
| defaultPath | java.lang.String | Le chemin par défaut. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Initialise une nouvelle instance de la classe [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Le chemin personnalisé de l'utilisateur (URL) enregistré dans le fichier HTML généré pour la source référencée. S'il n'est pas défini par l'utilisateur, DefaultPath sera utilisé. Par exemple, les données de la feuille seront enregistrées par l'utilisateur dans d:/sheet001.htm, l'URL utilisée dans le fichier HTML principal doit être \"d:/sheet001.htm\" ou tout autre chemin relatif valide pouvant être accédé par le fichier HTML principal.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


Le chemin par défaut (URL) enregistré dans le fichier HTML généré pour la source référencée. Par exemple, les données de la feuille enregistrées dans xxx\\_files/sheet001.htm, l'URL utilisée dans le fichier HTML principal devrait être comme \"src=\\\"xxx\\_files/sheet001.htm\\\"\"

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Obtient le flux d'entrée pour récupérer les données.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Obtient le type de ressource de chargement.

Voir [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Obtient le flux de sortie pour écrire les données enregistrées.

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


Le chemin personnalisé de l'utilisateur (URL) enregistré dans le fichier HTML généré pour la source référencée. S'il n'est pas défini par l'utilisateur, DefaultPath sera utilisé. Par exemple, les données de la feuille seront enregistrées par l'utilisateur dans d:/sheet001.htm, l'URL utilisée dans le fichier HTML principal doit être \"d:/sheet001.htm\" ou tout autre chemin relatif valide pouvant être accédé par le fichier HTML principal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Définit le flux d'entrée pour récupérer les données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Définit le type de ressource de chargement.

Voir [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Définit le flux de sortie pour écrire les données enregistrées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.io.OutputStream |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


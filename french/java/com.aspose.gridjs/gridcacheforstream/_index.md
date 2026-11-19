---
title: "GridCacheForStream"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Cette classe contient les opérations de cache pour GridJs."
type: docs
url: /fr/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Cette classe contient les opérations de cache pour GridJs. L'utilisateur doit implémenter sa propre logique métier pour le stockage basée sur celle-ci..
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implémentez cette méthode pour obtenir l'url du fichier depuis le cache. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Vérifie si le cache avec uid existe |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implémentez cette méthode pour charger le cache avec la clé uid, retourner le flux depuis le cache. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implémentez cette méthode pour sauvegarder le cache, enregistrer le flux dans le cache avec la clé uid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
```


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
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


Implémentez cette méthode pour obtenir l'url du fichier depuis le cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.String - L'URL du fichier
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


Vérifie si le cache avec uid existe

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
boolean - La valeur booléenne
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Implémentez cette méthode pour charger le cache avec la clé uid, retourner le flux depuis le cache.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


Implémentez cette méthode pour sauvegarder le cache, enregistrer le flux dans le cache avec la clé uid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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


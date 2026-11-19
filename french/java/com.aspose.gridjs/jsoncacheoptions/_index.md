---
title: "JsonCacheOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options de configuration pour le cache JSON dans GridJs."
type: docs
url: /fr/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Options de configuration pour le cache JSON dans GridJs. Contrôle le comportement du cache mémoire (L1) et du cache disque (L2).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Obtient si le cache disque doit être compressé avec Gzip (par défaut : true). |
| [getDiskPath()](#getDiskPath--) | Obtient le chemin du répertoire du cache disque. |
| [getDiskTtl()](#getDiskTtl--) | Obtient le TTL du cache disque, en minutes (par défaut : 1440). |
| [getEnable()](#getEnable--) | Obtient si le cache JSON est activé pour une réponse plus rapide. |
| [getEnableDisk()](#getEnableDisk--) | Obtient si le cache disque est activé (par défaut : true). |
| [getImplementation()](#getImplementation--) | Obtient l'implémentation personnalisée du cache JSON. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Obtient la taille maximale du cache disque en Mo (par défaut : 500 Mo). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Obtient le nombre maximal d'entrées dans le cache mémoire (par défaut : 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Obtient le TTL du cache mémoire, en minutes (par défaut : 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Définit si le cache disque doit être compressé avec Gzip (par défaut : true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Définit le chemin du répertoire du cache disque. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Définit le TTL du cache disque, en minutes (par défaut : 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Définit si le cache JSON est activé pour une réponse plus rapide. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Définit si le cache disque est activé (par défaut : true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Définit l'implémentation personnalisée du cache JSON. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Définit la taille maximale du cache disque en MB (par défaut : 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Définit le nombre maximal d'entrées dans le cache mémoire (par défaut : 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Définit le TTL du cache mémoire, en minutes (par défaut : 60). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonCacheOptions() {#JsonCacheOptions--}
```
public JsonCacheOptions()
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


Obtient si le cache disque doit être compressé avec Gzip (par défaut : true). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Obtient le chemin du répertoire du cache disque. Prend effet lorsque Enable = true et que le cache par défaut est utilisé. Par défaut : [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Obtient le TTL du cache disque, en minutes (par défaut : 1440). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Obtient si la mise en cache JSON doit être activée pour une réponse plus rapide. Lorsqu'elle est activée, GridJs mettra en cache le JSON généré et le réutilisera pour les requêtes suivantes. La valeur par défaut est false. Remarque : vous devez définir Implementation pour utiliser un stockage de cache personnalisé.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Obtient si le cache disque doit être activé (par défaut : true). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Obtient l'implémentation personnalisée du cache JSON. Si elle n'est pas définie, GridJs utilisera le cache mémoire + disque par défaut.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Obtient la taille maximale du cache disque en MB (par défaut : 500 MB). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Obtient le nombre maximal d'entrées dans le cache mémoire (par défaut : 1000). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Obtient le TTL du cache mémoire, en minutes (par défaut : 60). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Returns:**
long
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




### setCompressDisk(boolean value) {#setCompressDisk-boolean-}
```
public void setCompressDisk(boolean value)
```


Définit si le cache disque doit être compressé avec Gzip (par défaut : true). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Définit le chemin du répertoire du cache disque. Prend effet lorsque Enable = true et que le cache par défaut est utilisé. Par défaut : [FileCacheDirectory]/json\_cache

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Définit le TTL du cache disque, en minutes (par défaut : 1440). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Définit si la mise en cache JSON doit être activée pour une réponse plus rapide. Lorsqu'elle est activée, GridJs mettra en cache le JSON généré et le réutilisera pour les requêtes suivantes. La valeur par défaut est false. Remarque : vous devez définir Implementation pour utiliser un stockage de cache personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Définit si le cache disque doit être activé (par défaut : true). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Définit l'implémentation personnalisée du cache JSON. Si elle n'est pas définie, GridJs utilisera le cache mémoire + disque par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Définit la taille maximale du cache disque en MB (par défaut : 500 MB). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Définit le nombre maximal d'entrées dans le cache mémoire (par défaut : 1000). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Définit le TTL du cache mémoire, en minutes (par défaut : 60). Prend effet lorsque Enable = true et que le cache par défaut est utilisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | long |  |

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


---
title: "IGridJsService"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface des API d'opération de base utilisées dans les actions du contrôleur."
type: docs
url: /fr/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Représente l'interface des API d'opération de base utilisées dans les actions du contrôleur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Applique l'opération d'ajout d'image depuis un fichier local. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Applique l'opération d'ajout d'image depuis une URL distante. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Efface toutes les entrées du cache JSON (mémoire et disque). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Efface toutes les entrées du cache JSON appartenant à l'ID unique spécifié. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Applique l'opération de copie d'image. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Obtient la chaîne JSON du fichier par l'ID unique spécifié. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Écrire la chaîne JSON du classeur dans le flux |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Applique l'opération de téléchargement du fichier |
| [getFile(String fileid)](#getFile-java.lang.String-) | Obtenir le flux du fichier |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Obtenir le flux de l'image. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtient l'URL de l'image. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Écrit la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'identifiant unique spécifié vers le flux.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Récupère les données du tableau d'octets de l'objet OLE intégré. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applique l'opération de mise à jour. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
```


Applique l'opération d'ajout d'image depuis un fichier local.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | Le paramètre de chaîne JSON |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| flux de fichier | java.io.InputStream | Le flux de fichier de l'image |

**Returns:**
java.lang.String - Le résultat de la chaîne JSON
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Applique l'opération d'ajout d'image depuis une URL distante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | Le paramètre de chaîne JSON |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| flux de fichier | java.io.InputStream | Le flux de fichier de l'image |
| imageurl | java.lang.String | Spécifiez l'URL de l'image. |

**Returns:**
java.lang.String - Le résultat de la chaîne JSON
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public abstract boolean checkInCacheForCollaborative(String uid)
```


Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public abstract void clearAllJsonCache()
```


Efface toutes les entrées du cache JSON (mémoire et disque).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Efface toutes les entrées du cache JSON appartenant à l'identifiant unique spécifié. Appelez ceci après avoir modifié le fichier source hors bande afin que la prochaine requête régénère le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Applique l'opération de copie d'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | Le paramètre de chaîne JSON |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.String - Le résultat de la chaîne JSON
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Obtient la chaîne JSON du fichier par l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin du fichier |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Écrire la chaîne JSON du classeur dans le flux

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| filePath | java.lang.String | Le chemin du fichier |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| filePath | java.lang.String | Le chemin du fichier |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
```


Applique l'opération de téléchargement du fichier

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | Le paramètre JSON |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Le nom du fichier |

**Returns:**
java.lang.String - L'URL du fichier
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Obtenir le flux du fichier

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileid | java.lang.String | l'identifiant du fichier |

**Returns:**
java.io.InputStream - Le flux du fichier
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
```


Obtenir le flux de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| picid | java.lang.String | L'identifiant de l'image. |

**Returns:**
java.io.InputStream - Le flux de l'image
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String imageUrl(String baseURL, String picid, String uid)
```


Obtient l'URL de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseURL | java.lang.String | L'URL d'action de base. |
| picid | java.lang.String | L'identifiant de l'image. |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.String - L'URL de l'image
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | le nom de la feuille. |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Écrit la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'identifiant unique spécifié vers le flux..

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| sheetName | java.lang.String | Le nom de la feuille. |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public abstract String load(String uid, String filename)
```


Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |

**Returns:**
java.lang.String - La chaîne JSON
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
```


Récupère les données du tableau d'octets de l'objet OLE intégré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| sheetname | java.lang.String | Le nom de la feuille de calcul. |
| oleid | int | L'ID de l'objet OLE intégré. |
| label | java.lang.String | L'étiquette d'affichage de l'objet OLE intégré. |

**Returns:**
byte[] - Les données du tableau d'octets de l'objet OLE intégré .
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Applique l'opération de mise à jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | La chaîne au format JSON de l'opération de mise à jour. |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.String

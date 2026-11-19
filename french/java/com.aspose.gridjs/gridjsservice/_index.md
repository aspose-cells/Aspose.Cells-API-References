---
title: "GridJsService"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit les API d'opération de base utilisées dans les actions du contrôleur."
type: docs
url: /fr/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Fournit les API d'opération de base utilisées dans les actions du contrôleur.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | Le constructeur par défaut pour GridJsService |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Applique l'opération d'ajout d'image depuis un fichier local. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Applique l'opération d'ajout d'image depuis un fichier local. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Efface toutes les entrées du cache JSON (mémoire et disque). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Efface toutes les entrées du cache JSON appartenant à l'ID unique spécifié. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Applique l'opération de copie d'image. |
| [destroy()](#destroy--) | cette méthode est uniquement pour Java, elle implémente la méthode destroy dans DisposableBean, qui sera appelée automatiquement par Spring à la fin de la requête, en réalité elle appellera la méthode Dispose. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Obtient la chaîne JSON du fichier par l'ID unique spécifié. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Écrit la chaîne JSON du fichier dans le flux. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Applique l'opération de téléchargement du fichier |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Obtenir le flux du fichier |
| [getSettings()](#getSettings--) | Représente les paramètres du classeur. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Obtenir le flux de l'image. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtient l'URL de l'image. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Écrit la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'identifiant unique spécifié vers le flux.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Récupère les données du tableau d'octets de l'objet OLE intégré. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Représente les paramètres du classeur. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduit toutes les valeurs de chaîne vers la langue cible dans la feuille de calcul. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applique l'opération de mise à jour. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


Le constructeur par défaut pour GridJsService

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
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
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Applique l'opération d'ajout d'image depuis un fichier local.

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
public boolean checkInCacheForCollaborative(String uid)
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
public void clearAllJsonCache()
```


Efface toutes les entrées du cache JSON (mémoire et disque).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Efface toutes les entrées du cache JSON appartenant à l'identifiant unique spécifié. Appelez ceci après avoir modifié le fichier source hors bande afin que la prochaine requête régénère le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Applique l'opération de copie d'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | Le paramètre de chaîne JSON |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.String - Le résultat de la chaîne JSON
### destroy() {#destroy--}
```
public void destroy()
```


cette méthode est uniquement pour Java, elle implémente la méthode destroy dans DisposableBean, qui sera appelée automatiquement par Spring à la fin de la requête, en réalité elle appellera la méthode Dispose.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Obtient la chaîne JSON du fichier par l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin complet du fichier |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Écrit la chaîne JSON du fichier dans le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| filePath | java.lang.String | Le chemin complet du fichier |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Écrit la chaîne JSON du fichier dans le flux par l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| filePath | java.lang.String | Le chemin complet du fichier |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

### dispose() {#dispose--}
```
public void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


Obtenir le flux du fichier

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileid | java.lang.String | l'identifiant du fichier |

**Returns:**
java.io.InputStream - Le flux du fichier
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Représente les paramètres du classeur.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
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
public String imageUrl(String baseURL, String picid, String uid)
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
public StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public String load(String uid, String filename)
```


Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |

**Returns:**
java.lang.String - La chaîne JSON
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
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
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Représente les paramètres du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Traduit toutes les valeurs de chaîne vers la langue cible dans la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| sheetName | java.lang.String | Le nom de la feuille |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Le traducteur qui implémente la fonction translate |
| targetLanguage | java.lang.String | La langue cible |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Applique l'opération de mise à jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | java.lang.String | La chaîne au format JSON de l'opération de mise à jour. |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |

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


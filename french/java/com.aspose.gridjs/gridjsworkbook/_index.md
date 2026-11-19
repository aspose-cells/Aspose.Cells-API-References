---
title: "GridJsWorkbook"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la classe principale d'entrée pour GridJs"
type: docs
url: /fr/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Représente la classe principale d'entrée pour GridJs
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Crée une nouvelle instance de GridJsWorkbook. |
## Champs

| Champ | Description |
| --- | --- |
| [CacheImp](#CacheImp) | Implémentation personnalisée pour le stockage du cache, si vous souhaitez stocker le cache de manière flux, vous devez le configurer et l'implémenter. |
| [CalculateEngine](#CalculateEngine) | Implémentation personnalisée pour le moteur de calcul ,si vous souhaitez effectuer un calcul personnalisé, vous devez le définir et l'implémenter. |
| [PICTURE_TYPE](#PICTURE-TYPE) | valeur const pour le type de l'image |
| [UpdateMonitor](#UpdateMonitor) | Obtient/Définit le moniteur de mise à jour pour suivre l'opération de mise à jour |
## Méthodes

| Méthode | Description |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Applique (applique) toutes les opérations de rédaction dans le classeur en supprimant les formes de rédaction et leurs formes cibles ou en effaçant le contenu des plages de cellules cibles. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Vérifie si l'instance du classeur est dans le cache mémoire. Cette méthode s'applique uniquement au mode collaboratif. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Copie l'image ou la forme. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Obtient la chaîne du message d'erreur au format JSON. |
| [exportToJson()](#exportToJson--) | Obtient la chaîne JSON à partir des données en mémoire, le nom de fichier par défaut dans le JSON est : book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Obtient le répertoire de cache pour le stockage du fichier de feuille de calcul. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Obtient le format de chargement à partir de l'extension du fichier |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Obtenir le flux de l'image. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtient l'URL de l'image. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Récupère les données du tableau d'octets de l'objet OLE intégré. |
| [getSettings()](#getSettings--) | Représente les paramètres du classeur. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e feuille \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Génère un nouvel identifiant unique pour le cache de fichiers en utilisant le nom de fichier fourni. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement et le mot de passe d'ouverture. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importe le fichier Excel à partir du chemin du fichier. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Importe le fichier Excel à partir d'un flux de fichier. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement et le mot de passe d'ouverture. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Importe le fichier Excel à partir du chemin du fichier. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Importe le fichier Excel à partir du chemin du fichier et du mot de passe d'ouverture. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Importe le fichier Excel à partir d'une chaîne au format JSON. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Insère une image dans la feuille de calcul à partir d'un flux de fichier ou de l'URL (le flux de fichier ou l'URL doit être fourni) ou insère une forme, lorsque p.type est l'un des AutoShapeType |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Génère du JSON à partir du classeur en mémoire et l'écrit dans le flux spécifié. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON, et l'écrit dans le flux. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Récupère la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'identifiant unique spécifié, et l'écrit dans le flux. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Applique une mise à jour par lot aux données en mémoire. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Effectue une rédaction sur un fichier Excel basée sur un tableau d'opérations JSON. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Enregistre les données en mémoire dans le fichier cache avec le nom de fichier spécifié et définit également le mot de passe d'ouverture, le format d'enregistrement est basé sur l'extension du fichier. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Enregistre les données en mémoire dans le flux, basé sur le format du fichier d'origine. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Enregistre les données en mémoire dans le chemin du fichier, si le fichier a une extension, le format d'enregistrement est basé sur l'extension du fichier. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Enregistre les données en mémoire dans le flux, le format d'enregistrement est html |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Enregistre les données en mémoire dans le chemin du fichier, le format d'enregistrement est html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Enregistre les données en mémoire dans le flux, le format d'enregistrement est pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Enregistre les données en mémoire vers le chemin du fichier, le format d'enregistrement est pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Enregistre les données en mémoire vers le sream, le format d'enregistrement est xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Enregistre les données en mémoire vers le chemin du fichier, le format d'enregistrement est xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Définit le répertoire de cache pour stocker le fichier de feuille de calcul. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Définissez l'URL d'action de récupération de l'image de base depuis le contrôleur. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Définit InterruptMonitor pour l'opération de chargement. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Définit InterruptMonitor pour l'opération d'enregistrement. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Représente les paramètres du classeur. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Définit la transparence des formes de rédaction dans le classeur. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduit toutes les valeurs de chaîne vers la langue cible dans la feuille de calcul. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applique l'opération de mise à jour. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Crée une nouvelle instance de GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Implémentation personnalisée pour le stockage du cache, si vous souhaitez stocker le cache de manière flux, vous devez le configurer et l'implémenter.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Implémentation personnalisée pour le moteur de calcul ,si vous souhaitez effectuer un calcul personnalisé, vous devez le définir et l'implémenter.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


valeur const pour le type de l'image

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Obtient/Définit le moniteur de mise à jour pour suivre l'opération de mise à jour

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Applique (applique) toutes les opérations de rédaction dans le classeur en supprimant les formes de rédaction et leurs formes cibles ou en effaçant le contenu des plages de cellules cibles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| excelFilePath | java.lang.String | Le chemin du fichier Excel. |
| uid | java.lang.String | L'identifiant unique du classeur. Si nul ou vide, un nouvel uid sera généré à partir du chemin du fichier. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Copie l'image ou la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| p | java.lang.String | La chaîne JSON pour l'opération qui spécifie l'emplacement de la cellule, elle contient le nom de la feuille de calcul, la ligne supérieure gauche, la colonne supérieure gauche pour l'image ou la forme\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - La chaîne JSON de la nouvelle image copiée
### dispose() {#dispose--}
```
public void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Obtient la chaîne du message d'erreur au format JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| msg | java.lang.String | Le message d'erreur. |

**Returns:**
java.lang.String - La chaîne JSON.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Obtient la chaîne JSON à partir des données en mémoire, le nom de fichier par défaut dans le JSON est : book1.

**Returns:**
java.lang.String - La chaîne JSON.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1.. |

**Returns:**
java.lang.String - La chaîne JSON.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Obtient la chaîne JSON à partir des données en mémoire, définit le nom de fichier de sortie dans le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1.. |

**Returns:**
java.lang.StringBuilder - Le StringBuilder JSON.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Obtient le répertoire de cache pour le stockage du fichier de feuille de calcul. Si cela n'est pas défini, nous utiliserons la propriété statique de [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) ou [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Obtient le format de chargement à partir de l'extension du fichier

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extension | java.lang.String | L'extension du fichier, généralement commence par '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Obtenir le flux de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| picid | java.lang.String | L'identifiant de l'image. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Le flux de l'image
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Obtient l'URL de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| picid | java.lang.String | L'identifiant de l'image. |
| delimiter | java.lang.String | Le délimiteur de chaîne. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |

**Returns:**
java.lang.StringBuilder - Le StringBuilder de chaîne JSON
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Représente les paramètres du classeur.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \u9358\u71b7\ue750\u93c2\u56e6\u6b22\u935a?\* @return JSON \u701b\u6943\ue0c1\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Génère un nouvel identifiant unique pour le cache de fichiers en utilisant le nom de fichier fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\u6b22\u935a?\* @return JSON \u701b\u6943\ue0c1\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux de fichier | java.io.InputStream | Le flux du fichier Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Le LoadFormat du fichier Excel. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement et le mot de passe d'ouverture.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux de fichier | java.io.InputStream | Le flux du fichier Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Le LoadFormat du fichier Excel. |
| password | java.lang.String | Le mot de passe d'ouverture du fichier Excel. La valeur peut être nulle si aucun mot de passe n'est défini. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importe le fichier Excel à partir du chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le chemin complet du fichier. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Importe le fichier Excel à partir d'un flux de fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichier, s'il est défini sur null, il sera généré automatiquement. |
| flux de fichier | java.io.InputStream | Le flux du fichier Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Le LoadFormat du fichier Excel. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Importe le fichier Excel à partir d'un flux de fichier avec le format de chargement et le mot de passe d'ouverture.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichier, s'il est défini sur null, il sera généré automatiquement. |
| flux de fichier | java.io.InputStream | Le flux du fichier Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Le LoadFormat du fichier Excel. |
| password | java.lang.String | Le mot de passe d'ouverture du fichier Excel. La valeur peut être nulle si aucun mot de passe n'est défini |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Importe le fichier Excel à partir du chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichier, s'il est défini sur null, il sera généré automatiquement. |
| fileName | java.lang.String | Le chemin complet du fichier. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Importe le fichier Excel à partir du chemin du fichier et du mot de passe d'ouverture.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichier, s'il est défini sur null, il sera généré automatiquement. |
| fileName | java.lang.String | Le chemin complet du fichier. |
| password | java.lang.String | Le mot de passe d'ouverture du fichier Excel. La valeur peut être nulle si aucun mot de passe n'est défini. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Importe le fichier Excel à partir d'une chaîne au format JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| json | java.lang.String | La chaîne au format JSON. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Insère une image dans la feuille de calcul à partir d'un flux de fichier ou de l'URL (le flux de fichier ou l'URL doit être fourni) ou insère une forme, lorsque p.type est l'un des AutoShapeType

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichier |
| p | java.lang.String | La chaîne au format JSON pour l'opération qui spécifie l'emplacement de la cellule, le nom de la feuille de calcul, la ligne supérieure gauche, la colonne supérieure gauche pour l'image\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Le flux du fichier image |
| imageUrl | java.lang.String | L'URL du fichier image |

**Returns:**
java.lang.String - La chaîne au format JSON de l'image insérée
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Générer du JSON à partir du classeur en mémoire et l'écrire dans le flux spécifié. Met en cache éventuellement le JSON généré pour une récupération ultérieure plus rapide. Principales différences avec JsonToStreamByUid : - Cette méthode utilise l'état actuel du classeur en mémoire (champ wb) - JsonToStreamByUid recharge le classeur à partir des fichiers de cache .cells sur le disque - Utilisez cette méthode lorsque vous souhaitez exporter l'état actuel du classeur après des modifications - Utilisez JsonToStreamByUid lorsque vous devez régénérer le JSON à partir d'un état de fichier précédemment mis en cache Comportement de mise en cache (lorsqu'un uid est fourni) : - Vérifie le cache JSON avant de générer (mémoire L1 + disque L2) - En cas d'absence de cache, génère le JSON à partir du classeur en mémoire - Stocke le JSON généré dans le cache pour les requêtes futures

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de sortie où écrire les données JSON |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| nom de fichier | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Récupère la chaîne JSON du fichier depuis le cache en utilisant l'identifiant unique spécifié, définit le nom de fichier de sortie dans le JSON, et l'écrit dans le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Spécifie le nom de fichier dans le JSON. Si défini sur null, le nom de fichier par défaut est : book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Obtient la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'ID unique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| sheetName | java.lang.String | le nom de la feuille. |

**Returns:**
java.lang.StringBuilder - Le StringBuilder de chaîne JSON
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Récupère la chaîne JSON de la feuille spécifiée dans le fichier depuis le cache en utilisant l'identifiant unique spécifié, et l'écrit dans le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux qui sera écrit |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| sheetName | java.lang.String | le nom de la feuille. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Applique une mise à jour par lot aux données en mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| json | java.lang.String | La chaîne au format JSON de mise à jour. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


Effectue une rédaction sur un fichier Excel basée sur un tableau d'opérations JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| excelFilePath | java.lang.String | Le chemin du fichier Excel à masquer. |
| uid | java.lang.String | L'identifiant unique du classeur. Si nul ou vide, un nouvel uid sera généré à partir du chemin du fichier. |
| arrayOfRedactionOpr | java.lang.String[] | Un tableau de chaînes JSON représentant les opérations de masquage à appliquer. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Enregistre les données en mémoire dans le fichier cache avec le nom de fichier spécifié et définit également le mot de passe d'ouverture, le format d'enregistrement est basé sur l'extension du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | L'identifiant unique pour le cache de fichiers. |
| nom de fichier | java.lang.String | Le nom de fichier à enregistrer. |
| password | java.lang.String | Le mot de passe d'ouverture du fichier Excel. La valeur peut être nulle si aucun mot de passe n'est défini. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Enregistre les données en mémoire dans le flux, basé sur le format du fichier d'origine.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux à enregistrer. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Enregistre les données en mémoire dans le chemin du fichier, si le fichier a une extension, le format d'enregistrement est basé sur l'extension du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Le chemin du fichier à enregistrer. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Enregistre les données en mémoire dans le flux, le format d'enregistrement est html

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux à enregistrer. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Enregistre les données en mémoire dans le chemin du fichier, le format d'enregistrement est html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Le chemin du fichier à enregistrer. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Enregistre les données en mémoire dans le flux, le format d'enregistrement est pdf.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux à enregistrer. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Enregistre les données en mémoire vers le chemin du fichier, le format d'enregistrement est pdf.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Le chemin du fichier à enregistrer. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Enregistre les données en mémoire vers le sream, le format d'enregistrement est xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux à enregistrer. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Enregistre les données en mémoire vers le chemin du fichier, le format d'enregistrement est xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | java.lang.String | Le chemin du fichier à enregistrer. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Définit le répertoire de cache pour le stockage du fichier de feuille de calcul. Si cela n'est pas défini, nous utiliserons la propriété statique de [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) ou [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Définissez l'URL d'action de récupération de l'image de base depuis le contrôleur.

**Remarks**

Lorsque CacheImp est nul, nous devons définir ceci.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| baseImageURL | java.lang.String | L'URL d'action de récupération de l'image de base. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Définit InterruptMonitor pour l'opération de chargement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | L'instance InterruptMonitor. |
| calculateTimeoutMilliseconds | int | Le délai d'attente en millisecondes pour le chargement du fichier. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Définit InterruptMonitor pour l'opération d'enregistrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | L'instance InterruptMonitor. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Représente les paramètres du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Définit la transparence des formes de rédaction dans le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| excelFilePath | java.lang.String | Le chemin du fichier Excel. |
| uid | java.lang.String | L'identifiant unique du classeur. Si nul ou vide, un nouvel uid sera généré à partir du chemin du fichier. |
| isTransparent | boolean | Si vrai, définit la transparence à 0,89 (semi-transparente) ; si faux, définit la transparence à 1 (complètement opaque/invisible). |

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
java.lang.String - La chaîne au format JSON du résultat de mise à jour.
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


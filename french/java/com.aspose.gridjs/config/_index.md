---
title: "Config"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les paramètres statiques pour GridJs"
type: docs
url: /fr/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Représente tous les paramètres statiques pour GridJs
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Config()](#Config--) |  |
## Champs

| Champ | Description |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indique s'il faut utiliser un identifiant généré par le client au lieu de l'identifiant réel de la forme dans les opérations liées à la rédaction |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Obtient s'il faut optimiser automatiquement les performances de chargement pour les feuilles de calcul contenant de grandes cellules. |
| [getBaseRouteName()](#getBaseRouteName--) | Obtient le nom de la route de base pour l'URL du contrôleur GridJs. la valeur par défaut est "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Obtient le nombre maximal de colonnes par défaut pour une feuille de calcul vide. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Obtient le nombre maximal de lignes par défaut pour une feuille de calcul vide. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Obtient s'il faut activer le rendu de graphiques côté client. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Obtient le répertoire de cache pour le stockage du fichier de feuille de calcul. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Obtient s'il faut afficher la plage maximale qui inclut les données, le style, les cellules fusionnées et les formes. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Obtient s'il faut limiter le nombre total de formes/images affichés dans une feuille de calcul, si réglé sur true, GridJs limitera le nombre total de formes ou images affichées dans une feuille de calcul à MaxShapeOrImageCount, la valeur par défaut est true. |
| [getJsonCache()](#getJsonCache--) | Obtient les options de configuration du cache JSON. |
| [getLazyLoading()](#getLazyLoading--) | Obtient s'il faut charger uniquement la feuille de calcul active, la valeur par défaut est false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Obtient le nombre maximal de secondes d'expiration lors de l'enregistrement en PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Obtient le nombre total de formes ou images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Obtient la largeur ou hauteur maximale pour une forme ou une image, GridJs ignorera les formes ou images dont la largeur ou hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Obtient le nombre total de formes ou images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Obtient les destinations websocket préfixées par "/topic". la valeur par défaut est "/topic/opr". utilisé uniquement en mode collaboratif. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Obtient le répertoire de cache pour les images. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Obtient s'il faut vérifier si les images ont la même source, la valeur par défaut est true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Obtient s'il faut enregistrer le fichier HTML en tant qu'archive zip, la valeur par défaut est false. |
| [getShowChartSheet()](#getShowChartSheet--) | Obtient s'il faut afficher la feuille de calcul du graphique. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Obtient si l’on doit ignorer les formes qui sont invisibles pour l’interface utilisateur, la valeur par défaut est true. |
| [getUsePrintArea()](#getUsePrintArea--) | Obtient si l’on doit utiliser PageSetup.PrintArea pour la plage d’affichage de l’interface utilisateur lorsque la feuille de calcul possède le paramètre PageSetup pour PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Obtient si l’on doit prendre en charge l’édition collaborative, la valeur par défaut est false. |
| [isWasm()](#isWasm--) | Obtient si GridJs s’exécute à l’intérieur d’un hôte WebAssembly de navigateur au lieu d’un processus serveur. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Définit si l’on doit optimiser automatiquement les performances de chargement pour les feuilles de calcul contenant de grandes cellules. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Définit le nom de la route de base pour l'URL du contrôleur GridJs. la valeur par défaut est "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Définit si l’on doit prendre en charge l’édition collaborative, la valeur par défaut est false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Définit le nombre maximal de colonnes par défaut pour une feuille de calcul vide. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Définit le nombre maximal de lignes par défaut pour une feuille de calcul vide. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Définit si l’on doit activer le rendu de graphiques côté client. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Définit le répertoire de cache pour stocker le fichier de feuille de calcul. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Définit le dossier des polices |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Définit les dossiers de polices |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Définit si l’on doit afficher la plage maximale qui inclut les données, le style, les cellules fusionnées et les formes. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Définit si l’on doit limiter le nombre total de formes/images affichées dans une feuille de calcul, si défini sur true, GridJs limitera le nombre total de formes ou d’images affichées dans une feuille de calcul à MaxShapeOrImageCount. La valeur par défaut est true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Définit les options de configuration du cache JSON. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Définit si l’on doit charger uniquement la feuille de calcul active, la valeur par défaut est false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Définit le nombre maximal de secondes d’expiration lors de l’enregistrement au format PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Définit le nombre total de formes ou d’images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Définit la largeur ou la hauteur maximale pour une forme ou une image, GridJs ignorera la forme ou l’image dont la largeur ou la hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Définit le nombre total de formes ou d’images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Définit les destinations websocket préfixées par "/topic". La valeur par défaut est "/topic/opr". Utilisé uniquement en mode collaboratif. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Définit le répertoire de cache pour les images. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Définit si l’on doit vérifier si les images ont la même source, la valeur par défaut est true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Définit si l’on doit enregistrer le fichier HTML en tant qu’archive zip, la valeur par défaut est false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Définit si l’on doit afficher la feuille de calcul du graphique. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Définit s'il faut ignorer les formes qui sont invisibles dans l'UI, la valeur par défaut est true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Définit s'il faut utiliser PageSetup.PrintArea pour la plage d'affichage de l'UI lorsque la feuille de calcul possède le paramètre PageSetup pour PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | Définit si GridJs s'exécute dans un hôte WebAssembly de navigateur au lieu d'un processus serveur. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
```


Indique s'il faut utiliser un identifiant généré par le client au lieu de l'identifiant réel de la forme dans les opérations liées à la rédaction

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir ceci sur `true` effectuera une opération d'ajustement automatique de toutes les colonnes après le chargement, ce qui peut avoir un impact notable sur les performances.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir ceci sur `true` effectuera une opération d'ajustement automatique de toutes les lignes après le chargement, ce qui peut avoir un impact notable sur les performances.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Obtient s'il faut optimiser automatiquement les performances de chargement pour les feuilles de calcul contenant de grandes cellules. Il ignorera certains styles / bordures pour réduire le temps de chargement. La valeur par défaut est true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Obtient le nom de la route de base pour l'URL du contrôleur GridJs. la valeur par défaut est "/GridJs2".

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public static int getEmptySheetMaxCol()
```


Obtient le nombre maximal de colonnes par défaut pour une feuille de calcul vide. La valeur par défaut est 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Obtient le nombre maximal de lignes par défaut pour une feuille de calcul vide. La valeur par défaut est 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Obtient si le rendu des graphiques côté client est activé. Si défini sur false, GridJs reviendra uniquement aux images/formes de graphiques générées par le serveur. la valeur par défaut est true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Obtient le répertoire de cache pour le stockage du fichier de feuille de calcul. Nous devons le définir sur un chemin spécifique avant d'utiliser GridJs.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Obtient s'il faut afficher la plage maximale qui inclut les données, le style, les cellules fusionnées et les formes. Si la dernière ligne ou colonne contient des cellules sans valeur ni formule mais avec un style personnalisé, alors nous n'afficherons pas cette ligne/colonne lorsque cette valeur est true\u9286?\* La valeur par défaut est true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Obtient s'il faut limiter le nombre total de formes/images affichés dans une feuille de calcul, si réglé sur true, GridJs limitera le nombre total de formes ou images affichées dans une feuille de calcul à MaxShapeOrImageCount, la valeur par défaut est true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Obtient les options de configuration du cache JSON. Contrôle le comportement du cache mémoire (L1) et disque (L2) pour le JSON du classeur généré.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Obtient s'il faut charger uniquement la feuille de calcul active, la valeur par défaut est false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Obtient le nombre maximal de secondes d'expiration lors de l'enregistrement en PDF. La valeur par défaut est 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Obtient le nombre total de formes ou d'images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Obtient la largeur ou hauteur maximale pour une forme ou une image, GridJs ignorera la forme ou l'image dont la largeur ou la hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Obtient le nombre total de formes ou d'images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Obtient les destinations websocket préfixées par "/topic". la valeur par défaut est "/topic/opr". utilisé uniquement en mode collaboratif.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Obtient le répertoire de cache pour les images. (cela prend effet lorsque GridJsWorkbook.CacheImp est null) le chemin par défaut sera "\_piccache" à l'intérieur du FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Obtient s'il faut vérifier si les images ont la même source, la valeur par défaut est true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Obtient s'il faut enregistrer le fichier HTML en tant qu'archive zip, la valeur par défaut est false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Obtient s'il faut afficher la feuille de graphique. La valeur par défaut est false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Obtient si l’on doit ignorer les formes qui sont invisibles pour l’interface utilisateur, la valeur par défaut est true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Obtient s'il faut utiliser PageSetup.PrintArea pour la plage d'affichage de l'UI lorsque la feuille de calcul possède le paramètre PageSetup pour PrintArea. La valeur par défaut est false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public static boolean isCollaborative()
```


Obtient si l’on doit prendre en charge l’édition collaborative, la valeur par défaut est false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Obtient si GridJs s'exécute dans un hôte WebAssembly de navigateur au lieu d'un processus serveur. Lorsque true, aucun chemin FileCacheDirectory / disque / thread d'interruption n'est utilisé et le cache de fichiers doit provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm définit cela lors de la construction du service GridJs, de sorte qu'un seul Aspose.Cells.GridJs.dll serve les deux hôtes. la valeur par défaut est false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public static void setAutoFitColumnsOnLoad(boolean value)
```


Indique s'il faut ajuster automatiquement la largeur des colonnes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir ceci sur `true` effectuera une opération d'ajustement automatique de toutes les colonnes après le chargement, ce qui peut avoir un impact notable sur les performances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Indique s'il faut ajuster automatiquement la hauteur des lignes lors du chargement du fichier. La valeur par défaut est `false`. Avertissement : définir ceci sur `true` effectuera une opération d'ajustement automatique de toutes les lignes après le chargement, ce qui peut avoir un impact notable sur les performances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Définit s'il faut optimiser automatiquement les performances de chargement pour les feuilles de calcul contenant de grandes cellules. Il ignorera certains styles / bordures pour réduire le temps de chargement. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Définit le nom de la route de base pour l'URL du contrôleur GridJs. la valeur par défaut est "/GridJs2".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Définit si l’on doit prendre en charge l’édition collaborative, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Définit le nombre maximal de colonnes par défaut pour une feuille de calcul vide. La valeur par défaut est 15.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Définit le nombre maximal de lignes par défaut pour une feuille de calcul vide. La valeur par défaut est 12.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Définit si le rendu des graphiques côté client est activé. Si défini sur false, GridJs reviendra uniquement aux images/formes de graphiques générées par le serveur. la valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Définit le répertoire de cache pour le stockage du fichier de feuille de calcul. Nous devons le définir sur un chemin spécifique avant d'utiliser GridJs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Définit le dossier des polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolder | java.lang.String | Le dossier contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Définit les dossiers de polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Les dossiers contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Définit s'il faut afficher la plage maximale qui inclut les données, le style, les cellules fusionnées et les formes. Si la dernière ligne ou colonne contient des cellules sans valeur ni formule mais avec un style personnalisé, alors nous n'afficherons pas cette ligne/colonne lorsque cette valeur est true\u9286?\* La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Définit si l’on doit limiter le nombre total de formes/images affichées dans une feuille de calcul, si défini sur true, GridJs limitera le nombre total de formes ou d’images affichées dans une feuille de calcul à MaxShapeOrImageCount. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Définit les options de configuration du cache JSON. Contrôle le comportement du cache mémoire (L1) et du cache disque (L2) pour le JSON du classeur généré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Définit si l’on doit charger uniquement la feuille de calcul active, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Définit le nombre maximal de secondes d'expiration lors de l'enregistrement en PDF. La valeur par défaut est 10.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Définit le nombre total de formes ou d'images affichées dans la feuille active, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 100.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Définit la largeur ou la hauteur maximale pour une forme ou une image, GridJs ignorera la forme ou l'image dont la largeur ou la hauteur dépasse cette valeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 10000.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Définit le nombre total de formes ou d'images affichées dans le classeur, cela prend effet lorsque IslimitShapeOrImage=true. La valeur par défaut est 300.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Définit les destinations websocket préfixées par "/topic". La valeur par défaut est "/topic/opr". Utilisé uniquement en mode collaboratif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Définit le répertoire de cache pour les images. (cela prend effet lorsque GridJsWorkbook.CacheImp est nul) le chemin par défaut sera "\\_piccache" dans le FileCacheDirectory.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Définit si l’on doit vérifier si les images ont la même source, la valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Définit si l’on doit enregistrer le fichier HTML en tant qu’archive zip, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Définit s'il faut afficher la feuille de graphique. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Définit s'il faut ignorer les formes qui sont invisibles dans l'UI, la valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Définit s'il faut utiliser PageSetup.PrintArea pour la plage d'affichage UI lorsque la feuille possède le paramètre PageSetup pour PrintArea. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Définit si GridJs s'exécute dans un hôte WebAssembly de navigateur au lieu d'un processus serveur. Lorsque true, aucun chemin FileCacheDirectory / disque / thread d'interruption n'est utilisé et le cache de fichiers doit provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm définit cela lors de la construction du service GridJs, de sorte qu'un seul Aspose.Cells.GridJs.dll serve les deux hôtes. la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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


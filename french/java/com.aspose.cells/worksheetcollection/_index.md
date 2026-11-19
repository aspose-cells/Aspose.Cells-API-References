---
title: "WorksheetCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Encapsule une collection d’objets [Worksheet](../../com.aspose.cells/worksheet).

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute une feuille de calcul à la collection. |
| [add(int type)](#add-int-) | Ajoute une feuille de calcul à la collection. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Ajoute une feuille de calcul à la collection. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Copie un groupe de feuilles de calcul. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [clear()](#clear--) | Efface toutes les feuilles de calcul. |
| [clearPivottables()](#clearPivottables--) | Supprime les tableaux croisés dynamiques de la feuille de calcul. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [Worksheet](../../com.aspose.cells/worksheet) à l'index spécifié. |
| [get(String sheetName)](#get-java.lang.String-) | Obtient l'élément [Worksheet](../../com.aspose.cells/worksheet) avec le nom spécifié. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [getActiveSheetName()](#getActiveSheetName--) | Représente le nom de la feuille de calcul active lorsque le classeur est ouvert. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [getDxfs()](#getDxfs--) | Obtient les enregistrements de mise en forme différentielle maîtres. |
| [getExternalLinks()](#getExternalLinks--) | Représente les liens externes dans un classeur. |
| [getNamedRanges()](#getNamedRanges--) | Obtient toutes les plages nommées pré‑définies dans la feuille de calcul. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Obtient toutes les plages nommées pré‑définies dans la feuille de calcul. |
| [getNames()](#getNames--) | Obtient la collection de tous les objets Name dans la feuille de calcul. |
| [getOleSize()](#getOleSize--) | Obtient la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [getPivotCaches()](#getPivotCaches--) | Obtient tous les [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Obtient l'objet Range par nom pré‑défini. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Obtient le [Range](../../com.aspose.cells/range) par nom pré‑défini ou par nom de tableau |
| [getRevisionLogs()](#getRevisionLogs--) | Représente les journaux de révision. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Représente toutes les étiquettes de sensibilité. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Obtient la feuille de calcul par le nom de code. |
| [getTableStyles()](#getTableStyles--) | Obtient l'objet [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--). |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Obtient la liste des auteurs de commentaires en fil. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Obtient la liste des volets de tâches. |
| [getWebExtensions()](#getWebExtensions--) | Obtient la liste des volets de tâches. |
| [getXmlMaps()](#getXmlMaps--) | Obtient les cartes XML dans le classeur. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [insert(int index, int sheetType)](#insert-int-int-) | Insérer une feuille de calcul. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Insérer une feuille de calcul. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Indique si toutes les connexions sont rafraîchies à l'ouverture du fichier dans MS Excel. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Rafraîchir tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé. |
| [refreshPivotTables()](#refreshPivotTables--) | Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Ajoute la fonction addin au classeur. |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Ajoute la fonction addin au classeur. |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à un index spécifié. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Supprime l'élément à un nom spécifié. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Représente le nom de la feuille de calcul active lorsque le classeur est ouvert. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Indique si toutes les connexions sont rafraîchies à l'ouverture du fichier dans MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Définit les cartes XML dans le classeur. |
| [sortNames()](#sortNames--) | Trie les noms définis. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Échange les deux feuilles. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Ajoute une feuille de calcul à la collection.

**Returns:**
int - index de l'objet [Worksheet](../../com.aspose.cells/worksheet).
### add(int type) {#add-int-}
```
public int add(int type)
```


Ajoute une feuille de calcul à la collection.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Type de feuille. |

**Returns:**
int - index de l'objet [Worksheet](../../com.aspose.cells/worksheet).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Ajoute une feuille de calcul à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Copie un groupe de feuilles de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Les feuilles de calcul source. |
| destSheetNames | java.lang.String[] | Les noms des feuilles copiées. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index de la feuille de calcul source. |

**Returns:**
int - index de l'objet [Worksheet](../../com.aspose.cells/worksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul source. |

**Returns:**
int - index de l'objet [Worksheet](../../com.aspose.cells/worksheet).
### clear() {#clear--}
```
public void clear()
```


Efface toutes les feuilles de calcul.

**Remarks**

Un classeur doit contenir une feuille de calcul.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Supprime les tableaux croisés dynamiques de la feuille de calcul.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | L'adresse de la plage. |
| sheetIndex | int | L’indice de la feuille. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Crée un objet [Range](../../com.aspose.cells/range) à partir d'une adresse de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | L'adresse de la plage. |
| sheetIndex | int | L’indice de la feuille. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Obtient l'élément [Worksheet](../../com.aspose.cells/worksheet) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Obtient l'élément [Worksheet](../../com.aspose.cells/worksheet) avec le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Représente l'index de la feuille de calcul active lorsque le classeur est ouvert.

**Remarks**

L'index de la feuille commence à zéro.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Représente le nom de la feuille de calcul active lorsque le classeur est ouvert.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul.

**Remarks**

Une nouvelle propriété ne peut pas être ajoutée à la liste des propriétés de document intégrées. Vous ne pouvez que récupérer une propriété intégrée et modifier sa valeur. La liste suivante présente les noms des propriétés intégrées :

Title

Sujet

Auteur

Mots-clés

Commentaires

Modèle

Dernier auteur

Numéro de révision

Nom de l'application

Date de la dernière impression

Date de création

Heure du dernier enregistrement

Temps total d'édition

Nombre de pages

Nombre de mots

Nombre de caractères

Sécurité

Catégorie

Format

Gestionnaire

Entreprise

Nombre d'octets

Nombre de lignes

Nombre de paragraphes

Nombre de diapositives

Nombre de notes

Nombre de diapositives masquées

Nombre de clips multimédias

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Obtient les enregistrements de mise en forme différentielle maîtres.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Représente les liens externes dans un classeur.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Obtient toutes les plages nommées pré‑définies dans la feuille de calcul.

**Returns:**
com.aspose.cells.Range[] - Un tableau d'objets Range. Si la référence du Name défini est externe ou possède plusieurs plages, aucun objet Range ne sera renvoyé pour ce Name.

Renvoie null si la plage nommée n'existe pas.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Obtient toutes les plages nommées pré‑définies dans la feuille de calcul.

**Returns:**
com.aspose.cells.Range[] - Un tableau d'objets Range.

Renvoie null si la plage nommée n'existe pas.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Obtient la collection de tous les objets Name dans la feuille de calcul.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Obtient la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole.

**Remarks**

Null signifie qu'aucun réglage de taille ole n'est défini.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Obtient tous les [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Obtient l'objet Range par nom pré‑défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rangeName | java.lang.String | Nom de la plage. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Renvoie null si la plage nommée n'existe pas.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Obtient le [Range](../../com.aspose.cells/range) par nom pré‑défini ou par nom de tableau

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rangeName | java.lang.String | Nom de la plage ou nom de la table. |
| currentSheetIndex | int | L'index de la feuille. -1 représente global . |
| includeTable | boolean | Indique s'il faut vérifier toutes les tables. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Représente les journaux de révision.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Représente toutes les étiquettes de sensibilité.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Obtient la feuille de calcul par le nom de code.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| codeName | java.lang.String | Nom de code de la feuille de calcul. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Obtient l'objet [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--).

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Obtient la liste des auteurs de commentaires en fil.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Obtient la liste des volets de tâches.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Obtient la liste des volets de tâches.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Obtient les cartes XML dans le classeur.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Insérer une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la feuille |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Le type de feuille. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Insérer une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la feuille |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Le type de feuille. |
| sheetName | java.lang.String | Le nom de la feuille. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Indique si toutes les connexions sont rafraîchies à l'ouverture du fichier dans MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Rafraîchir tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Workbook.RefreshAll(). Cette méthode sera supprimée 12 mois plus tard depuis avril 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | L'option de rafraîchissement de la source de données des tableaux croisés dynamiques. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Ajoute la fonction addin au classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| id | int | ID des données contenant les fonctions addin, peut être obtenu lors du premier appel de [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) pour le même fichier addin. |
| functionName | java.lang.String | le nom de la fonction addin |

**Returns:**
java.lang.String - URL du fichier addin contenant les fonctions addin
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Ajoute la fonction addin au classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| addInFile | java.lang.String | le fichier contenant les fonctions addin |
| functionName | java.lang.String | le nom de la fonction addin |
| lib | boolean | si le fichier addin fourni se trouve dans le répertoire ou sous‑répertoire de la bibliothèque Workbook Add‑In. Ce drapeau prend effet et fait une différence lorsque le addInFile fourni est un chemin relatif : true indique que le chemin est relatif à la bibliothèque Add‑In et false indique que le chemin est relatif à ce classeur. |

**Returns:**
int - ID des données qui contiennent la fonction addin fournie
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'élément à un index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | La valeur d'index de l'élément à supprimer. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Supprime l'élément à un nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de l'élément à supprimer. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Représente l'index de la feuille de calcul active lorsque le classeur est ouvert.

**Remarks**

L'index de la feuille commence à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Représente le nom de la feuille de calcul active lorsque le classeur est ouvert.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole.

**Remarks**

Cette méthode est généralement utilisée pour ajuster la taille d'affichage dans un fichier ppt ou doc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | Indice de ligne de départ. |
| endRow | int | Indice de ligne de fin. |
| startColumn | int | Indice de colonne de départ. |
| endColumn | int | Indice de colonne de fin. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole.

**Remarks**

Null signifie qu'aucun réglage de taille ole n'est défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Indique si toutes les connexions sont rafraîchies à l'ouverture du fichier dans MS Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Définit les cartes XML dans le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Trie les noms définis.

**Remarks**

Si vous créez un grand nombre de plages nommées dans le fichier Excel, veuillez appeler cette méthode après la création de toutes les plages nommées et avant l'enregistrement.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Échange les deux feuilles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex1 | int | La première feuille de calcul. |
| sheetIndex2 | int | La deuxième feuille de calcul. |

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


---
title: "SqlScriptSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du sql."
type: docs
url: /fr/java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

Représente les options d'enregistrement du sql.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | Crée des options pour enregistrer le fichier sql. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | Insère une ligne vide entre chaque donnée. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | Vérifie toutes les données pour trouver le type de données des colonnes. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | Vérifie si le nom de la table existe avant de créer. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getColumnTypeMap()](#getColumnTypeMap--) | Obtient la correspondance des types de colonnes pour différentes bases de données. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getCreateTable()](#getCreateTable--) | Indique si l'exportation du sql de création de table est activée. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExportArea()](#getExportArea--) | Obtient la plage d'exportation. |
| [getExportAsString()](#getExportAsString--) | Indique si l'exportation de toutes les données en tant que valeur chaîne est activée. |
| [getIdName()](#getIdName--) | Obtient le nom de la colonne id. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getOperatorType()](#getOperatorType--) | Obtient le type d'opérateur du sql. |
| [getPrimaryKey()](#getPrimaryKey--) | Représente la colonne qui est la clé primaire du tableau de données. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSeparator()](#getSeparator--) | Obtient le séparateur de caractères du script sql. |
| [getSheetIndexes()](#getSheetIndexes--) | Représente les index des feuilles exportées. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getStartId()](#getStartId--) | Obtient l'identifiant de départ. |
| [getTableName()](#getTableName--) | Obtient le nom de la table. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hasHeaderRow()](#hasHeaderRow--) | Indique si la plage contient une ligne d'en-tête. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | Insère une ligne vide entre chaque donnée. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | Vérifie toutes les données pour trouver le type de données des colonnes. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | Vérifie si le nom de la table existe avant de créer. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | Définit la correspondance des types de colonnes pour différentes bases de données. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | Indique si l'exportation du sql de création de table est activée. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Définit la plage d'exportation. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Indique si l'exportation de toutes les données en tant que valeur chaîne est activée. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indique si la plage contient une ligne d'en-tête. |
| [setIdName(String value)](#setIdName-java.lang.String-) | Définit le nom de la colonne id. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setOperatorType(int value)](#setOperatorType-int-) | Définit le type d'opérateur du sql. |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | Représente la colonne qui est la clé primaire du tableau de données. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSeparator(char value)](#setSeparator-char-) | Définit le séparateur de caractères du script sql. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Représente les index des feuilles exportées. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setStartId(int value)](#setStartId-int-) | Définit l'identifiant de départ. |
| [setTableName(String value)](#setTableName-java.lang.String-) | Définit le nom de la table. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


Crée des options pour enregistrer le fichier sql.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


Insère une ligne vide entre chaque donnée.

**Remarks**

Si [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\\#getSeparator--) est '\\n' , il est préférable de définir cette propriété sur true pour améliorer la lisibilité.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Returns:**
java.lang.String
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


Vérifie toutes les données pour trouver le type de données des colonnes.

**Remarks**

La valeur par défaut est false, nous ne vérifions que la première ligne pour des raisons de performance. Si cette propriété est true et que les colonnes contiennent des types de valeurs mixtes, le type des colonnes sera texte.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


Vérifie si le nom de la table existe avant de créer.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Rendre le classeur vide après l'enregistrement du fichier.

**Returns:**
boolean
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


Obtient la correspondance des types de colonnes pour différentes bases de données.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


Indique si l'exportation du sql de création de table est activée.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Obtient la plage d'exportation.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Indique si l'exportation de toutes les données en tant que valeur chaîne est activée.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


Obtient le nom de la colonne id.

**Remarks**

Si cette propriété est définie , une colonne sera insérée avec une valeur entière à incrémentation automatique.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


Obtient le type d'opérateur du sql.

Voir [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


Représente la colonne qui est la clé primaire du tableau de données.

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de fichier d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Obtient le séparateur de caractères du script sql.

**Remarks**

Ne peut être que ' ' ou '\\n'. Si le

**Returns:**
char
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Représente les index des feuilles exportées.

**Returns:**
int[]
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Returns:**
boolean
### getStartId() {#getStartId--}
```
public int getStartId()
```


Obtient l'identifiant de départ.

**Remarks**

Ne fonctionne que lorsque [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) est défini.

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


Obtient le nom de la table.

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Indique si la plage contient une ligne d'en-tête.

**Returns:**
boolean
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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


Insère une ligne vide entre chaque donnée.

**Remarks**

Si [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\\#getSeparator--) est '\\n' , il est préférable de définir cette propriété sur true pour améliorer la lisibilité.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


Vérifie toutes les données pour trouver le type de données des colonnes.

**Remarks**

La valeur par défaut est false, nous ne vérifions que la première ligne pour des raisons de performance. Si cette propriété est true et que les colonnes contiennent des types de valeurs mixtes, le type des colonnes sera texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


Vérifie si le nom de la table existe avant de créer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendre le classeur vide après l'enregistrement du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


Définit la correspondance des types de colonnes pour différentes bases de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


Indique si l'exportation du sql de création de table est activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Définit la plage d'exportation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Indique si l'exportation de toutes les données en tant que valeur chaîne est activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indique si la plage contient une ligne d'en-tête.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


Définit le nom de la colonne id.

**Remarks**

Si cette propriété est définie , une colonne sera insérée avec une valeur entière à incrémentation automatique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


Définit le type d'opérateur du sql.

Voir [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


Représente la colonne qui est la clé primaire du tableau de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Définit le séparateur de caractères du script sql.

**Remarks**

Ne peut être que ' ' ou '\\n'. Si le

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Représente les index des feuilles exportées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int[] |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


Définit l'identifiant de départ.

**Remarks**

Ne fonctionne que lorsque [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) est défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


Définit le nom de la table.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Définit le rappel d’avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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


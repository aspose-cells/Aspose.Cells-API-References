---
title: "SettableGlobalizationSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation de GlobalizationSettings qui permet à l'utilisateur de définir/modifier des textes prédéfinis."
type: docs
url: /fr/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Implémentation de GlobalizationSettings qui permet à l'utilisateur de définir/modifier des textes prédéfinis.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compare deux valeurs de chaîne selon certaines règles de collation. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Obtient le nom de l'étiquette "(All)" dans le tableau croisé dynamique. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Obtient la chaîne d'affichage pour la valeur booléenne d'une cellule |
| [getChartSettings()](#getChartSettings--) | Obtient les paramètres de mondialisation pour le graphique. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforme la chaîne en un objet comparable selon certaines règles de collation. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Obtient le nom de l'étiquette "Column Labels" dans le tableau croisé dynamique. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Obtient le séparateur pour les éléments des données de ligne du tableau dans la formule. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Obtient le nom du titre de commentaire dépendant de la langue selon le type de titre de commentaire. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Obtient le nom de l'en-tête du champ de la zone de valeurs dans le tableau croisé dynamique. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Obtient le nom de feuille par défaut pour l'ajout automatique d'une feuille de calcul. |
| [getEmptyDataName()](#getEmptyDataName--) | Obtient le nom de l'étiquette "(blank)" dans le tableau croisé dynamique. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Obtient la valeur de chaîne d'affichage pour la valeur d'erreur de la cellule |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Obtient le nom du total général de la fonction. |
| [getListSeparator()](#getListSeparator--) | Obtient le séparateur pour la liste, les paramètres de la fonction, ...etc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Obtient le nom de l'étiquette "(Multiple Items)" dans le tableau croisé dynamique. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Obtient le nom de l'étiquette "Grand Total" dans le tableau croisé dynamique. |
| [getPivotSettings()](#getPivotSettings--) | Obtient les paramètres de mondialisation pour le tableau croisé dynamique. |
| [getPivotTotalName()](#getPivotTotalName--) | Obtient le nom de l'étiquette "Total" dans le tableau croisé dynamique. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Obtient le nom de protection dans le tableau croisé dynamique. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Obtient le nom de l'étiquette "Row Labels" dans le tableau croisé dynamique. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Obtient le séparateur pour les lignes dans les données de tableau dans la formule. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Obtient le nom du type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) dans le tableau croisé dynamique. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Obtient le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Obtient le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Obtient le nom du type des lignes de tableau qui comprend la région de données du tableau référencé. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Obtient le nom du type des lignes de tableau qui comprend l'en-tête du tableau. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Obtient le nom du type des lignes de tableau qui comprend la ligne totale du tableau référencé. |
| [getTotalName(int functionType)](#getTotalName-int-) | Obtient le nom total de la fonction spécifique. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Définit la valeur de chaîne d'affichage pour la valeur booléenne de la cellule |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Définit les paramètres de mondialisation pour le graphique. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Définit le séparateur des éléments dans les données de ligne du tableau dans la formule. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Obtient le nom du titre de commentaire dépendant de la langue selon le type de titre de commentaire. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Définit le nom du total général d'une fonction spécifique. |
| [setListSeparator(char c)](#setListSeparator-char-) | Définit le séparateur pour la liste, les paramètres de la fonction, ...etc. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Définit le texte dépendant de la locale pour le nom intégré avec le texte de nom standard fourni. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Définit le nom de fonction dépendant de la locale correspondant au nom de fonction standard fourni. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Définit les paramètres de mondialisation pour le tableau croisé dynamique. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Définit le séparateur des lignes dans les données de tableau dans la formule. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Définit le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Définit le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Définit le nom du type des lignes de tableau qui comprend la région de données du tableau référencé. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Définit le nom du type des lignes de tableau qui comprend l'en-tête du tableau. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Définit le nom du type des lignes de tableau qui comprend la ligne totale du tableau référencé. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Définit le nom du total d'une fonction spécifique. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Compare deux valeurs de chaîne selon certaines règles de collation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| v1 | java.lang.String | la première chaîne |
| v2 | java.lang.String | la deuxième chaîne |
| ignoreCase | boolean | indique s'il faut ignorer la casse lors de la comparaison des valeurs |

**Returns:**
int - Entier qui indique la relation lexicale entre les deux comparands
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Obtient le nom de l'étiquette "(All)" dans le tableau croisé dynamique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode GlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois plus tard à compter de décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de l\u00e9tiquette "(All)"
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Obtient la chaîne d'affichage pour la valeur booléenne d'une cellule

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| bv | boolean | valeur booléenne |

**Returns:**
java.lang.String - Par défaut, renvoie "TRUE" pour la valeur vraie et "FALSE" pour la valeur fausse.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Obtient les paramètres de mondialisation pour le graphique.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transforme la chaîne en un objet comparable selon certaines règles de collation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| v | java.lang.String | La valeur String doit être comparée avec d'autres. |
| ignoreCase | boolean | indique s'il faut ignorer la casse lors de la comparaison des valeurs |

**Returns:**
java.lang.Comparable - L'objet peut être utilisé pour comparer ou trier des valeurs de chaîne
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Obtient le nom de l'étiquette "Column Labels" dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom des libellés de colonne
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Obtient le séparateur pour les éléments des données de ligne du tableau dans la formule.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Obtient le nom du titre de commentaire dépendant de la langue selon le type de titre de commentaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). type de titre de commentaire |

**Returns:**
java.lang.String - nom du titre de commentaire dépendant de la locale
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Obtient le nom de l'en-tête du champ de la zone de valeurs dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de l'en-tête du champ de données
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Obtient le nom de feuille par défaut pour l'ajout automatique d'une feuille de calcul. La valeur par défaut est "Sheet".

**Remarks**

Le nom de la feuille ajoutée automatiquement (par exemple via [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) sera le nom spécifié suivi d'un numéro de séquence. Par exemple, un utilisateur allemand peut vouloir que le nom de la feuille soit "Tabellenblatt2" au lieu de "Sheet2". L'utilisateur peut alors implémenter cette méthode pour renvoyer "Tabellenblatt".

**Returns:**
java.lang.String - le nom de feuille par défaut pour l'ajout automatique d'une feuille de calcul
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Obtient le nom de l'étiquette "(blank)" dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom des données vides
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Obtient la valeur de chaîne d'affichage pour la valeur d'erreur de la cellule

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| err | java.lang.String | valeurs d'erreur telles que \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - Par défaut, renvoie la valeur d'erreur elle-même
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Obtient le nom du total général de la fonction.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Le type de fonction. |

**Returns:**
java.lang.String - Le nom du total général de la fonction.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Obtient le séparateur pour la liste, les paramètres de la fonction, ...etc.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) texte du nom intégré. |

**Returns:**
java.lang.String - Texte dépendant de la locale. La locale a été spécifiée par le Workbook pour lequel ces paramètres sont utilisés.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) nom de fonction. |

**Returns:**
java.lang.String - Nom de fonction dépendant de la locale. La locale a été spécifiée par le Workbook pour lequel ces paramètres sont utilisés.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Obtient le nom de l'étiquette "(Multiple Items)" dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de l'étiquette "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Obtient le nom de l'étiquette "Grand Total" dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de l'étiquette "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Obtient les paramètres de mondialisation pour le tableau croisé dynamique.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Obtient le nom de l'étiquette "Total" dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs ou plus dans la zone de données.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de l'étiquette "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Obtient le nom de protection dans le tableau croisé dynamique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetTextOfProtectedName(string). Cette propriété sera supprimée 12 mois plus tard à compter de décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de protection du tableau croisé dynamique
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Obtient le nom de l'étiquette "Row Labels" dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom des libellés de ligne
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Obtient le séparateur pour les lignes dans les données de tableau dans la formule.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Texte dépendant de la langue du nom intégré. La langue a été spécifiée par le classeur pour lequel ces paramètres sont utilisés. |

**Returns:**
java.lang.String - Texte standard (locale en-US).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Nom de fonction dépendant de la langue. La langue a été spécifiée par le classeur pour lequel ces paramètres sont utilisés. |

**Returns:**
java.lang.String - Nom de fonction standard (locale en-US).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Nom du style de police dépendant de la langue pour En-tête/Pied de page. |

**Returns:**
java.lang.String - Nom de style de police anglais standard (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Obtient le nom du type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) dans le tableau croisé dynamique.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Cette propriété sera supprimée 12 mois après décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Le type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Le nom du type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Obtient le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé.

**Returns:**
java.lang.String - le nom du type des lignes de tableau
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Obtient le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé.

**Returns:**
java.lang.String - le nom du type des lignes de tableau
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Obtient le nom du type des lignes de tableau qui constitue la région de données du tableau référencé. La valeur par défaut est "Data", ainsi dans la formule "\#Data" représente la région de données du tableau.

**Returns:**
java.lang.String - le nom du type des lignes de tableau
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Obtient le nom du type des lignes de tableau qui constitue l'en-tête du tableau. La valeur par défaut est "Headers", ainsi dans la formule "\#Headers" représente l'en-tête du tableau.

**Returns:**
java.lang.String - le nom du type des lignes de tableau
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Obtient le nom du type des lignes de tableau qui comprend la ligne totale du tableau référencé.

**Returns:**
java.lang.String - le nom du type des lignes de tableau
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Obtient le nom total de la fonction spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Le type de fonction. |

**Returns:**
java.lang.String - Le nom total de la fonction.
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




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Définit la valeur de chaîne d'affichage pour la valeur booléenne de la cellule

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| bv | boolean | valeur booléenne |
| name | java.lang.String | valeur chaîne du booléen |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Définit les paramètres de mondialisation pour le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Définit le séparateur des éléments dans les données de ligne du tableau dans la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | char | le séparateur spécifié |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Obtient le nom du titre de commentaire dépendant de la langue selon le type de titre de commentaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). type de titre de commentaire |
| name | java.lang.String | Nom du titre du commentaire dépendant de la langue |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Définit le nom du total général d'une fonction spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Le type de fonction. |
| name | java.lang.String | Le nom du total général de la fonction. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Définit le séparateur pour la liste, les paramètres de la fonction, ...etc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | char | le séparateur spécifié |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Définit le texte dépendant de la locale pour le nom intégré avec le texte de nom standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Texte du nom standard (locale en-US) du nom intégré. |
| localName | java.lang.String | Texte du nom dépendant de la locale |
| bidirectional | boolean | Indique si le texte du nom local doit être mappé automatiquement au texte du nom standard. Si vrai, le texte du nom local sera mappé automatiquement au texte du nom standard, de sorte que l'utilisateur n'ait pas besoin d'appeler [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) de nouveau pour la même paire de noms standard et local. |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Définit le nom de fonction dépendant de la locale correspondant au nom de fonction standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) nom de fonction. |
| localName | java.lang.String | Nom de fonction dépendant de la locale |
| bidirectional | boolean | Indique si le nom de fonction local doit être mappé automatiquement au nom de fonction standard. Si vrai, le nom local sera mappé automatiquement au nom standard, de sorte que l'utilisateur n'ait pas besoin d'appeler [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) de nouveau pour la même paire de noms standard et local. |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Définit les paramètres de mondialisation pour le tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Définit le séparateur des lignes dans les données de tableau dans la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | char | le séparateur spécifié |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Nom de fonction dépendant de la locale |
| standardName | java.lang.String | Standard(en-US locale) nom de fonction. |
| bidirectional | boolean | Indique si le texte du nom standard doit être mappé automatiquement au texte du nom local. Si vrai, le texte du nom standard sera mappé automatiquement au texte du nom local, de sorte que l'utilisateur n'ait pas besoin d'appeler [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) de nouveau pour la même paire de noms standard et local. |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Nom de fonction dépendant de la locale |
| standardName | java.lang.String | Standard(en-US locale) nom de fonction. |
| bidirectional | boolean | Indique si le nom de fonction standard doit être mappé automatiquement au nom de fonction local. Si vrai, le nom standard sera mappé automatiquement au nom local, de sorte que l'utilisateur n'ait pas besoin d'appeler [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) de nouveau pour la même paire de noms standard et local. |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Nom du style de police dépendant de la langue pour En-tête/Pied de page. |
| standardName | java.lang.String | Standard(en-US locale) nom de fonction. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Définit le nom du type des lignes de tableau qui comprend toutes les lignes du tableau référencé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | le nom du type des lignes de tableau |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Définit le nom du type des lignes de tableau qui comprend la ligne actuelle du tableau référencé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | le nom du type des lignes de tableau |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Définit le nom du type des lignes de tableau qui comprend la région de données du tableau référencé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | le nom du type des lignes de tableau |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Définit le nom du type des lignes de tableau qui comprend l'en-tête du tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | le nom du type des lignes de tableau |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Définit le nom du type des lignes de tableau qui comprend la ligne totale du tableau référencé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | le nom du type des lignes de tableau |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Définit le nom du total d'une fonction spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Le type de fonction. |
| name | java.lang.String | Le nom total de la fonction. |

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


---
title: "PivotTableCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de tous les objets Tableau croisé dynamique sur la feuille de calcul spécifiée."
type: docs
url: /fr/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Représente la collection de tous les objets Tableau croisé dynamique sur la feuille de calcul spécifiée.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Ajoute un nouveau tableau croisé dynamique basé sur un autre tableau croisé dynamique. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Ajoute un nouveau tableau croisé dynamique basé sur un autre tableau croisé dynamique. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Ajoute un nouveau tableau croisé dynamique à la ligne et à la colonne spécifiées de la feuille de calcul. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Ajoute un nouveau tableau croisé dynamique. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Ajoute un nouvel objet Tableau Croisé Dynamique à la collection avec plusieurs plages de consolidation comme source de données. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Ajoute un nouvel objet Tableau Croisé Dynamique à la collection avec plusieurs plages de consolidation comme source de données. |
| [clear()](#clear--) | Efface tous les tableaux croisés dynamiques. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient le rapport de tableau croisé dynamique par indice. |
| [get(int row, int column)](#get-int-int-) | Obtient le [PivotTable](../../com.aspose.cells/pivottable) situé dans la cellule. |
| [get(String name)](#get-java.lang.String-) | Obtient le rapport de tableau croisé dynamique par le nom du tableau croisé dynamique. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Supprime le tableau croisé dynamique spécifié et supprime les données du tableau croisé dynamique. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Supprime le tableau croisé dynamique spécifié. |
| [removeAt(int index)](#removeAt-int-) | Supprime le tableau croisé dynamique à l'indice spécifié et supprime les données du tableau croisé dynamique. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Supprime le tableau croisé dynamique à l'indice spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Ajoute un nouveau tableau croisé dynamique basé sur un autre tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Le tableau croisé dynamique source. |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau tableau croisé dynamique ajouté.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Ajoute un nouveau tableau croisé dynamique basé sur un autre tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Le tableau croisé dynamique source. |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau tableau croisé dynamique ajouté.
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
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | int | L'indice de ligne basé sur zéro du coin supérieur gauche de la destination du tableau croisé dynamique. |
| colonne | int | L'indice de colonne basé sur zéro du coin supérieur gauche de la destination du tableau croisé dynamique. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Ajoute un nouveau tableau croisé dynamique à la ligne et à la colonne spécifiées de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| ligne | int | L'indice de ligne basé sur zéro du coin supérieur gauche de la destination du tableau croisé dynamique. |
| colonne | int | L'indice de colonne basé sur zéro du coin supérieur gauche de la destination du tableau croisé dynamique. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Options de création du tableau croisé dynamique. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice dans cette liste de tableaux croisés dynamiques.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela économisera de la mémoire. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après octobre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela économisera de la mémoire. |
| isXlsClassic | boolean | Indique si l'ajout d'un tableau croisé dynamique classique d'Excel 97-2003. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| cellName | java.lang.String | Le nom de la cellule du coin supérieur gauche pour la destination du tableau croisé dynamique. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Ajoute un nouveau tableau croisé dynamique moderne (depuis Excel 2007) à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| cellName | java.lang.String | Le nom de la cellule du coin supérieur gauche pour la destination du tableau croisé dynamique. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Les options de création du tableau croisé dynamique. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | Les données pour le nouveau cache de tableau croisé dynamique. |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice dans cette liste de tableaux croisés dynamiques.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Ajoute un nouveau tableau croisé dynamique avec la mise en page et le style hérités d'Excel 97-2003.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après septembre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | Les données pour le nouveau cache de tableau croisé dynamique. |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela économisera de la mémoire. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Ajoute un nouveau tableau croisé dynamique.

**Remarks**

NOTE: Cette méthode est obsolète. Elle est équivalente à appeler PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) avec `NewPivotTableOptions.IsXlsClassic = true`. Veuillez utiliser la surcharge PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) à la place. Cette méthode sera supprimée 12 mois après octobre 2026. Nous nous excusons pour tout inconvénient.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| cellule | java.lang.String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a déjà utilisé cette source de données. Si la propriété est vraie, cela permettra d'économiser de la mémoire lorsque la même source de données est regroupée dans un seul cache de tableau croisé dynamique. |
| isXlsClassic | boolean | Indique si l'ajout d'un tableau croisé dynamique classique d'Excel 97-2003. |

**Returns:**
int - L'indice du nouveau cache ajouté.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Ajoute un nouvel objet Tableau Croisé Dynamique à la collection avec plusieurs plages de consolidation comme source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String[] | Les multiples plages de consolidation, telles que \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Indique si un champ de page unique est créé automatiquement. Si vrai, le paramètre suivant pageFields sera ignoré |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Les éléments du champ de page du tableau croisé dynamique. |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | java.lang.String | Le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau tableau croisé dynamique ajouté.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Ajoute un nouvel objet Tableau Croisé Dynamique à la collection avec plusieurs plages de consolidation comme source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | java.lang.String[] | Les multiples plages de consolidation, telles que \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Indique si un champ de page unique est créé automatiquement. Si vrai, le paramètre suivant pageFields sera ignoré. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Les éléments du champ de page du tableau croisé dynamique. |
| destCellName | java.lang.String | destCellName Le nom du nouveau rapport de tableau croisé dynamique. |
| tableName | java.lang.String | le nom du nouveau rapport de tableau croisé dynamique. |

**Returns:**
int - L'indice du nouveau tableau croisé dynamique ajouté.
### clear() {#clear--}
```
public void clear()
```


Efface tous les tableaux croisés dynamiques.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


Obtient le rapport de tableau croisé dynamique par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Obtient le [PivotTable](../../com.aspose.cells/pivottable) situé dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int |  |
| colonne | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Obtient le rapport de tableau croisé dynamique par le nom du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
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




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Supprime le tableau croisé dynamique spécifié et supprime les données du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Supprime le tableau croisé dynamique spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| keepData | boolean | Indique s'il faut conserver les données du tableau croisé dynamique |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime le tableau croisé dynamique à l'indice spécifié et supprime les données du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de position dans la collection de tableaux croisés dynamiques |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Supprime le tableau croisé dynamique à l'indice spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de position dans la collection de tableaux croisés dynamiques |
| keepData | boolean | Indique s'il faut conserver les données du tableau croisé dynamique |

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


---
title: "Cellule"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une seule cellule de classeur."
type: docs
url: /fr/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Encapsule l'objet qui représente une seule cellule de classeur.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Calcule la formule de la cellule. |
| [characters(int startIndex, int length)](#characters-int-int-) | Renvoie un objet Characters qui représente une plage de caractères dans le texte de la cellule. |
| [containsExternalLink()](#containsExternalLink--) | Indique si cette cellule contient un lien externe. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Copie les données d'une cellule source. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule. |
| [equals(Object obj)](#equals-java.lang.Object-) | Vérifie si cet objet fait référence à la même cellule qu'un autre. |
| [getArrayRange()](#getArrayRange--) | Obtient la plage de tableau si la formule de la cellule est une formule de tableau. |
| [getBoolValue()](#getBoolValue--) | Obtient la valeur booléenne contenue dans la cellule. |
| [getCharacters()](#getCharacters--) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient le numéro de colonne (indexé à zéro) de la cellule. |
| [getComment()](#getComment--) | Obtient le commentaire de cette cellule. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Obtient le résultat du formatage conditionnel. |
| [getDateTimeValue()](#getDateTimeValue--) | Obtient la valeur DateTime contenue dans la cellule. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Obtient toutes les cellules dont la formule fait référence directement à cette cellule. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Obtient toutes les cellules dont le résultat calculé dépend de cette cellule. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Obtient la valeur chaîne formatée de cette cellule selon le style d'affichage de la cellule. |
| [getDisplayStyle()](#getDisplayStyle--) | Obtient le style d'affichage de cette cellule. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Obtient le style d'affichage de cette cellule. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Obtient le style d'affichage de cette cellule. |
| [getDoubleValue()](#getDoubleValue--) | Obtient la valeur double contenue dans la cellule. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Obtient l'image intégrée dans la cellule. |
| [getFloatValue()](#getFloatValue--) | Obtient la valeur float contenue dans la cellule. |
| [getFormatConditions()](#getFormatConditions--) | Obtient les conditions de format qui s'appliquent à cette cellule. |
| [getFormula()](#getFormula--) | Obtient une formule de la [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Obtient la formule de cette cellule. |
| [getFormulaLocal()](#getFormulaLocal--) | Obtenez la formule formatée selon la locale de la cellule. |
| [getHeightOfValue()](#getHeightOfValue--) | Obtient la hauteur de la valeur en unités de pixels. |
| [getHtmlString()](#getHtmlString--) | Obtient la chaîne html qui contient des données et certains formats dans cette cellule. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Obtient la chaîne html qui contient des données et certains formats dans cette cellule. |
| [getIntValue()](#getIntValue--) | Obtient la valeur entière contenue dans la cellule. |
| [getLeafs()](#getLeafs--) | Obtenez toutes les cellules qui font référence à cette cellule directement et qui doivent être mises à jour lorsque cette cellule est modifiée. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Obtenez toutes les cellules qui seront mises à jour lorsque cette cellule est modifiée. |
| [getMergedRange()](#getMergedRange--) | Renvoie un objet [Range](../../com.aspose.cells/range) qui représente une plage fusionnée. |
| [getName()](#getName--) | Obtient le nom de la cellule. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Représente le type de catégorie du format numérique de cette cellule. |
| [getPicture()](#getPicture--) | Obtient une instance [Picture](../../com.aspose.cells/picture) pour représenter l'image intégrée dans cette cellule ou null s'il n'y a aucune image intégrée pour cette cellule. |
| [getPrecedents()](#getPrecedents--) | Obtient toutes les références apparaissant dans la formule de cette cellule. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Obtient tous les antécédents (référence aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul. |
| [getR1C1Formula()](#getR1C1Formula--) | Obtient une formule R1C1 de la [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Obtient la valeur riche de la cellule. |
| [getRow()](#getRow--) | Obtient le numéro de ligne (indexé à zéro) de la cellule. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Obtient l'index du style partagé de la cellule dans le pool de styles. |
| [getStringValue()](#getStringValue--) | Obtient la valeur chaîne contenue dans la cellule. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Obtient la valeur chaîne selon une stratégie de formatage spécifique. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Obtient la valeur de la cellule sous forme de chaîne sans aucun format. |
| [getStyle()](#getStyle--) | Obtient le style de la cellule. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Si checkBorders est vrai, vérifiez si les bordures des autres cellules affecteront le style de cette cellule. |
| [getTable()](#getTable--) | Obtient le tableau qui contient cette cellule. |
| [getType()](#getType--) | Représente le type de valeur de la cellule. |
| [getValidation()](#getValidation--) | Obtient la validation appliquée à cette cellule. |
| [getValidationValue()](#getValidationValue--) | Obtient la valeur de la validation appliquée à cette cellule. |
| [getValue()](#getValue--) | Obtient la valeur contenue dans cette cellule. |
| [getWidthOfValue()](#getWidthOfValue--) | Obtient la largeur de la valeur en pixels. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul parente. |
| [hasCustomFunction()](#hasCustomFunction--) | Vérifie s'il existe une fonction personnalisée (fonction non prise en charge) dans la formule de cette cellule. |
| [hasCustomStyle()](#hasCustomStyle--) | Indique si cette cellule possède des paramètres de style personnalisés (différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondants). |
| [hashCode()](#hashCode--) | Servir de fonction de hachage pour un type particulier. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Insère des caractères dans la cellule. |
| [isArrayFormula()](#isArrayFormula--) | Indique si la formule de la cellule est une formule matricielle. |
| [isArrayHeader()](#isArrayHeader--) | Indique que la formule de la cellule est une formule matricielle et qu'elle est la première cellule du tableau. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Indique si la cellule est définie comme case à cocher. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Indique si la formule de la cellule est une formule matricielle dynamique (vrai) ou une formule matricielle héritée (faux). |
| [isErrorValue()](#isErrorValue--) | Vérifie si la valeur de cette cellule est une erreur. |
| [isFormula()](#isFormula--) | Indique si la cellule spécifiée contient une formule. |
| [isInArray()](#isInArray--) | Indique si la formule de la cellule est une formule matricielle. |
| [isInTable()](#isInTable--) | Indique si cette cellule fait partie d'une formule de tableau. |
| [isMerged()](#isMerged--) | Vérifie si une cellule fait partie d'une plage fusionnée ou non. |
| [isNumericValue()](#isNumericValue--) | Indique si la valeur de cette cellule est numérique (int, double et datetime). |
| [isRichText()](#isRichText--) | Indique si la valeur chaîne de cette cellule est un texte richement formaté. |
| [isSharedFormula()](#isSharedFormula--) | Indique si la formule de la cellule fait partie d'une formule partagée. |
| [isStyleSet()](#isStyleSet--) | Indique si le style de la cellule est défini. |
| [isTableFormula()](#isTableFormula--) | Indique si cette cellule fait partie d'une formule de tableau. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Place une valeur booléenne dans la cellule. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Place une valeur DateTime dans la cellule. |
| [putValue(double doubleValue)](#putValue-double-) | Place une valeur double dans la cellule. |
| [putValue(int intValue)](#putValue-int-) | Place une valeur entière dans la cellule. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Place une valeur d'objet dans la cellule. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Place une valeur chaîne dans la cellule. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Insère une valeur dans la cellule, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Supprimer la formule de tableau. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Remplacer le texte de la cellule avec des options. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Définit une formule de tableau (formule de tableau héritée saisie via CTRL+SHIFT+ENTER dans MS Excel) pour une plage de cellules. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Définit une formule de tableau pour une plage de cellules. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Définit une formule de tableau pour une plage de cellules. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Définit une formule de tableau pour une plage de cellules. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Définit le format de texte enrichi de la cellule. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Indique si la cellule est définie comme case à cocher. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Définit l'image intégrée dans la cellule. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Définit une formule de la [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Définir la formule et la valeur de la formule. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Définir la formule et la valeur(résultat calculé) de la formule. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Définir la formule et la valeur(résultat calculé) de la formule. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Définir la formule et la valeur(résultat calculé) de la formule. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Obtenez la formule formatée selon la locale de la cellule. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Définit la chaîne html qui contient des données et certains formats dans cette cellule. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Définit une formule R1C1 de la [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Définit des formules partagées pour une plage de cellules. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Définit une formule pour une plage de cellules. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Définit des formules partagées pour une plage de cellules. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Définit des formules partagées pour une plage de cellules. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Définit le style de la cellule. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Appliquer la propriété modifiée du style à la cellule. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Appliquer le style de la cellule en fonction des indicateurs. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Créer un tableau de données à une variable pour la plage donnée à partir de cette cellule. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Créer un tableau de données à deux variables pour la plage donnée à partir de cette cellule. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Créer un tableau de données à une variable pour la plage donnée à partir de cette cellule. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Créer un tableau de données à deux variables pour la plage donnée à partir de cette cellule. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit la valeur contenue dans cette cellule. |
| [toJson()](#toJson--) | Convertir la [Cell](../../com.aspose.cells/cell) en données de structure JSON. |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Calcule la formule de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options de calcul |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Renvoie un objet Characters qui représente une plage de caractères dans le texte de la cellule.

**Remarks**

Cette méthode ne fonctionne que sur une cellule avec une valeur de chaîne.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index du début du caractère. |
| length | int | Le nombre de caractères. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Copie les données d'une cellule source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objet source [Cell](../../com.aspose.cells/cell). |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | un autre objet cellule |

**Returns:**
booléen - vrai si deux objets cellule font référence à la même cellule.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Vérifie si cet objet fait référence à la même cellule qu'un autre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | un autre objet |

**Returns:**
booléen - vrai si deux objets font référence à la même cellule.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Obtient la plage de tableau si la formule de la cellule est une formule de tableau.

**Remarks**

S'applique uniquement lorsque la formule de la cellule est une formule de tableau.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Obtient la valeur booléenne contenue dans la cellule.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule.

**Returns:**
com.aspose.cells.FontSetting[] - Tous les objets Characters
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indicateur | boolean | Indique si le style de tableau doit être appliqué à la cellule lorsque celle‑ci se trouve dans le tableau. |

**Returns:**
com.aspose.cells.FontSetting[] - Tous les objets Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient le numéro de colonne (indexé à zéro) de la cellule.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Obtient le commentaire de cette cellule.

**Remarks**

S'il n'y a aucun commentaire appliqué à la cellule, renvoie null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Obtient le résultat du formatage conditionnel.

**Remarks**

Renvoie null si aucun formatage conditionnel n'est appliqué à cette cellule,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Obtient la valeur DateTime contenue dans la cellule.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Obtient toutes les cellules dont la formule fait référence directement à cette cellule.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indique s'il faut vérifier les formules dans d'autres feuilles de calcul. |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Obtient toutes les cellules dont le résultat calculé dépend de cette cellule.

**Remarks**

Pour utiliser cette méthode, veuillez vous assurer que le classeur a été configuré avec la valeur true pour [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) et qu'il a été entièrement calculé avec ce paramètre. S'il n'existe aucune référence de formule à cette cellule, null sera renvoyé.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| recursive | boolean | Indique si la méthode renvoie les dépendants qui ne font pas référence directement à cette cellule mais à d'autres feuilles de celle‑ci. |

**Returns:**
java.util.Iterator - Énumérateur pour parcourir tous les dépendants (objets Cell).
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Obtient la valeur chaîne formatée de cette cellule selon le style d'affichage de la cellule.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Obtient le style d'affichage de cette cellule.

**Remarks**

Identique à l'utilisation de [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) pour [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). Ainsi, cette méthode vérifiera et ajustera les bordures supérieure/basse/gauche/droite de cette cellule en fonction du style ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) de ses cellules adjacentes, mais ne vérifiera pas les cellules fusionnées, et ne vérifiera pas le style d'affichage des cellules adjacentes.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Obtient le style d'affichage de cette cellule.

**Remarks**

Si l'indicateur spécifié est false, alors c'est équivalent à [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). Sinon, c'est équivalent à l'utilisation de [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) pour [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indique s'il faut vérifier les bordures des cellules fusionnées. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Obtient le style d'affichage de cette cellule.

**Remarks**

Si cette cellule est également affectée par d'autres paramètres tels que le formatage conditionnel, les objets de liste, etc., le style d'affichage peut différer de [getStyle()](../../com.aspose.cells/cell\#getStyle--).

Pour les indicateurs d'ajustement des bordures selon les cellules adjacentes, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) indiquent s'il faut vérifier et combiner les bordures inférieure/ supérieure/ droite/ gauche des cellules adjacentes situées à gauche/droite/haut/bas de celle‑ci.

Pour des raisons de performance et de compatibilité, certains énumérations sont utilisées pour désigner des opérations spéciales :

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Veuillez noter que la vérification des bordures/styles des cellules adjacentes, en particulier les styles d'affichage, est un processus gourmand en temps. S'il n'est pas nécessaire d'obtenir les bordures pour le style retourné, utiliser [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) pour désactiver le traitement des cellules adjacentes améliorera les performances. Lors de l'obtention des bordures des cellules adjacentes à partir des styles définis uniquement sur ces cellules (sans définir [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), les performances peuvent également être meilleures car la vérification du style d'affichage d'une cellule est également coûteuse en temps.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indique quelles bordures doivent être vérifiées et ajustées en fonction des bordures des cellules adjacentes. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtient la valeur double contenue dans la cellule.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Obtient l'image intégrée dans la cellule.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Obtient la valeur float contenue dans la cellule.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Obtient les conditions de format qui s'appliquent à cette cellule.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Renvoie l'objet [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection).
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient une formule de la [Cell](../../com.aspose.cells/cell).

**Remarks**

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Obtient la formule de cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - la formule de cette cellule.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Obtenez la formule formatée selon la locale de la cellule.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Obtient la hauteur de la valeur en unités de pixels.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Obtient la chaîne html qui contient des données et certains formats dans cette cellule.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Obtient la chaîne html qui contient des données et certains formats dans cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| html5 | boolean | Indique si la valeur est compatible avec html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Obtient la valeur entière contenue dans la cellule.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Obtenez toutes les cellules qui font référence à cette cellule directement et qui doivent être mises à jour lorsque cette cellule est modifiée.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir tous les dépendants dans la chaîne de calcul. Cette propriété sera supprimée 12 mois après, depuis mai 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.util.Iterator - Énumérateur pour énumérer tous les dépendants (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Obtenez toutes les cellules qui seront mises à jour lorsque cette cellule est modifiée.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.GetDependentsInCalculation(bool) pour obtenir tous les dépendants dans la chaîne de calcul. Cette propriété sera supprimée 12 mois après, depuis mai 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| recursive | boolean | Indique si cela renvoie les feuilles qui ne font pas référence directement à cette cellule mais qui font référence à d'autres feuilles de cette cellule |

**Returns:**
java.util.Iterator - Énumérateur pour énumérer tous les dépendants (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Renvoie un objet [Range](../../com.aspose.cells/range) qui représente une plage fusionnée.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la cellule.

**Remarks**

Un nom de cellule comprend sa lettre de colonne et son numéro de ligne. Par exemple, le nom d'une cellule à la ligne 0 et à la colonne 0 est A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Représente le type de catégorie du format numérique de cette cellule.

Voir [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Lorsque le modèle de formatage d'une cellule est combiné avec des modèles de formatage conditionnel, le type retourné correspond à la partie utilisée pour la valeur actuelle de cette cellule. Par exemple, si le modèle de formatage de cette cellule est "\#,\#\#0;(\#,\#\#0);"-";@", alors lorsque la valeur de la cellule est numérique et différente de 0, le type retourné est [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER) ; lorsque la valeur de la cellule est 0 ou non numérique, le type retourné est [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Obtient une instance [Picture](../../com.aspose.cells/picture) pour représenter l'image intégrée dans cette cellule ou null s'il n'y a aucune image intégrée pour cette cellule.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Obtient toutes les références apparaissant dans la formule de cette cellule.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Obtient tous les antécédents (référence aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul.

**Remarks**

Cette méthode ne fonctionne que si [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) est vrai pour le classeur et que le classeur a été entièrement calculé. Si cette cellule n'est pas une formule ou ne fait référence à aucune autre cellule, null sera retourné.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - Énumérateur pour énumérer toutes les références (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Obtient une formule R1C1 de la [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Obtient la valeur riche de la cellule.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Obtient le numéro de ligne (indexé à zéro) de la cellule.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Obtient l'index du style partagé de la cellule dans le pool de styles.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtient la valeur chaîne contenue dans la cellule. Si le type de cette cellule est string, alors la valeur chaîne elle‑même est retournée. Pour les autres types de cellules, la valeur chaîne formatée (formatée avec le style spécifié de cette cellule) sera retournée. La valeur de cellule formatée est identique à ce que vous pouvez obtenir depuis Excel en copiant une cellule en texte (par exemple en copiant la cellule vers un éditeur de texte ou en l'exportant en CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Obtient la valeur chaîne selon une stratégie de formatage spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). La stratégie formatée. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Obtient la valeur de la cellule sous forme de chaîne sans aucun format.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, l'utilisateur doit obtenir l'objet valeur et le formater selon le type de valeur et les exigences spécifiques. Cette propriété sera supprimée 12 mois après, depuis décembre 2020. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtient le style de la cellule.

**Remarks**

Pour modifier le style de la cellule, veuillez appeler la méthode Cell.SetStyle() après avoir modifié l'objet style retourné. Cette méthode est identique à [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) avec la valeur true pour le paramètre.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Si checkBorders est vrai, vérifiez si les bordures des autres cellules affecteront le style de cette cellule.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| checkBorders | boolean | Vérifier les bordures des autres cellules |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Obtient le tableau qui contient cette cellule.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Représente le type de valeur de la cellule.

Voir [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Obtient la validation appliquée à cette cellule.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Obtient la valeur de la validation appliquée à cette cellule.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur contenue dans cette cellule.

**Remarks**

Type possible :

null,

Boolean,

DateTime,

Double,

Integer

String.

Pour une valeur int, elle peut être renvoyée sous forme d'un objet Integer ou d'un objet Double. Et il n'y a aucune garantie que la valeur renvoyée reste toujours du même type d'objet.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Obtient la largeur de la valeur en pixels.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient la feuille de calcul parente.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Vérifie s'il existe une fonction personnalisée (fonction non prise en charge) dans la formule de cette cellule.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indique si cette cellule possède des paramètres de style personnalisés (différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondants).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servir de fonction de hachage pour un type particulier.

**Returns:**
int - Un code de hachage pour l'objet Cell actuel.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Insérez quelques caractères dans la cellule. Si la cellule est richement formatée, cette méthode peut conserver le formatage d'origine.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |
| texte | java.lang.String | Texte inséré. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indique si la formule de la cellule est une formule matricielle.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Indique que la formule de la cellule est une formule matricielle et qu'elle est la première cellule du tableau.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Indique si la cellule est définie comme case à cocher.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Indique si la formule de la cellule est une formule matricielle dynamique (vrai) ou une formule matricielle héritée (faux).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Vérifie si la valeur de cette cellule est une erreur.

**Remarks**

S'applique également aux cellules de formule pour vérifier si le résultat calculé est une erreur.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indique si la cellule spécifiée contient une formule.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Indique si la formule de la cellule est une formule matricielle.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.IsArrayFormula pour vérifier si la formule de la cellule est une formule de tableau. Cette propriété sera supprimée 12 mois plus tard, depuis mai 2018. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Indique si cette cellule fait partie d'une formule de tableau.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.IsTableFormula pour vérifier si la formule de la cellule fait partie d'une formule de tableau. Cette propriété sera supprimée 12 mois plus tard, depuis mai 2018. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Vérifie si une cellule fait partie d'une plage fusionnée ou non.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Indique si la valeur de cette cellule est numérique (int, double et datetime).

**Remarks**

S'applique également aux cellules de formule pour vérifier le résultat calculé

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Indique si la valeur chaîne de cette cellule est un texte richement formaté.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Indique si la formule de la cellule fait partie d'une formule partagée.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule possède le format de cellule par défaut.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Indique si cette cellule fait partie d'une formule de tableau.

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




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Place une valeur booléenne dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Place une valeur DateTime dans la cellule.

**Remarks**

Définir une valeur DateTime pour une cellule ne signifie pas que la cellule sera automatiquement formatée en date/heure. La valeur DateTime est conservée comme une valeur numérique dans le modèle de données à la fois de MS Excel et d'Aspose.Cells. Le fait que la valeur numérique soit interprétée comme une simple valeur numérique ou comme une date/heure dépend du format numérique appliqué à cette cellule. Si cette cellule n'est pas formatée en date/heure, elle sera affichée comme une valeur numérique même si vous avez saisi une DateTime.

**Example**

Cet exemple montre comment définir une valeur DateTime dans une cellule et la faire afficher en tant que date/heure.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Valeur d'entrée |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Place une valeur double dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| doubleValue | double | Valeur d'entrée |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Place une valeur entière dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| intValue | int | Valeur d'entrée |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Place une valeur d'objet dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objectValue | java.lang.Object | valeur d'entrée |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Place une valeur chaîne dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |
| isConverted | boolean | True : converti en un autre type de données si approprié. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Insère une valeur dans la cellule, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |
| isConverted | boolean | True : converti en un autre type de données si approprié. |
| setStyle | boolean | True : définir le format numérique dans le style de la cellule lors de la conversion en un autre type de données |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Supprimer la formule de tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | boolean | True représente la conversion de la formule de tableau en formule normale. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Remplacer le texte de la cellule avec des options.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValue | java.lang.String | Valeur de chaîne à remplacer |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Les options de remplacement |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Définit une formule de tableau (formule de tableau héritée saisie via CTRL+SHIFT+ENTER dans MS Excel) pour une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formule de tableau. |
| rowNumber | int | Nombre de lignes pour remplir le résultat de la formule de tableau. |
| columnNumber | int | Nombre de colonnes pour remplir le résultat de la formule de tableau. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Définit une formule de tableau pour une plage de cellules.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Cette propriété sera supprimée 12 mois plus tard depuis décembre 2019. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formule de tableau. |
| rowNumber | int | Nombre de lignes pour remplir le résultat de la formule de tableau. |
| columnNumber | int | Nombre de colonnes pour remplir le résultat de la formule de tableau. |
| isR1C1 | boolean | si la formule est une formule R1C1 |
| isLocal | boolean | si la formule est formatée selon la locale |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Définit une formule de tableau pour une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formule de tableau. |
| rowNumber | int | Nombre de lignes pour remplir le résultat de la formule de tableau. |
| columnNumber | int | Nombre de colonnes pour remplir le résultat de la formule de tableau. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Définit une formule de tableau pour une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formule de tableau. |
| rowNumber | int | Nombre de lignes pour remplir le résultat de la formule de tableau. |
| columnNumber | int | Nombre de colonnes pour remplir le résultat de la formule de tableau. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |
| valeurs | java.lang.Object[][] | valeurs pour ces cellules avec la formule de tableau donnée |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Définit le format de texte enrichi de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Tous les objets Characters. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Indique si la cellule est définie comme case à cocher.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

**Remarks**

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S’il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "\\#SPILL!". Mais pour ce type de situation nous retournons toujours la plage complète dans laquelle cette formule devrait se déverser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | l’expression de la formule |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options pour analyser la formule. L’option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| calculateValue | boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage déversée. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

**Remarks**

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S’il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "\\#SPILL!". Mais pour ce type de situation nous retournons toujours la plage complète dans laquelle cette formule devrait se déverser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | l’expression de la formule |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options pour analyser la formule. L’option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| valeurs | java.lang.Object[][] | valeurs (résultats calculés) pour ces cellules avec la formule de tableau dynamique donnée |
| calculateRange | boolean | si calculer la plage déversée pour cette formule de tableau dynamique. Si le paramètre "values" n’est pas nul et que ce drapeau est false, alors la hauteur de la plage déversée sera values.Length et la largeur sera values[0].Length. |
| calculateValue | boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage déversée lorsque "values" est null ou que l’élément correspondant dans "values" pour une cellule est null. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible.

**Remarks**

la plage renvoyée peut ne pas être identique à celle réelle dans laquelle cette formule de tableau dynamique se déverse. S’il y a des cellules non vides dans la plage, la formule sera définie uniquement pour la cellule actuelle et marquée comme "\\#SPILL!". Mais pour ce type de situation nous retournons toujours la plage complète dans laquelle cette formule devrait se déverser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | l’expression de la formule |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options pour analyser la formule. L’option "Parse" sera ignorée et la formule sera toujours analysée immédiatement |
| valeurs | java.lang.Object[][] | valeurs (résultats calculés) pour ces cellules avec la formule de tableau dynamique donnée |
| calculateRange | boolean | si calculer la plage déversée pour cette formule de tableau dynamique. Si le paramètre "values" n’est pas nul et que ce drapeau est false, alors la hauteur de la plage déversée sera values.Length et la largeur sera values[0].Length. |
| calculateValue | boolean | si calculer cette formule de tableau dynamique pour ces cellules dans la plage déversée lorsque "values" est null ou que l’élément correspondant dans "values" pour une cellule est null. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Les options pour le calcul de la formule. Généralement, pour des considérations de performance, la propriété [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\\#getRecursive--) devrait être false. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Définit l'image intégrée dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Définit une formule de la [Cell](../../com.aspose.cells/cell).

**Remarks**

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Définir la formule et la valeur de la formule.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetFormula(string,FormulaParseOptions,object). Cette propriété sera supprimée 12 mois plus tard depuis décembre 2019. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule. |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |
| valeur | java.lang.Object | La valeur de la formule. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Définir la formule et la valeur(résultat calculé) de la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Définir la formule et la valeur(résultat calculé) de la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |
| valeur | java.lang.Object | La valeur (résultat calculé) de la formule. |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Définir la formule et la valeur(résultat calculé) de la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule. |
| valeur | java.lang.Object | La valeur (résultat calculé) de la formule. |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Obtenez la formule formatée selon la locale de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Définit la chaîne html qui contient des données et certains formats dans cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Définit une formule R1C1 de la [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Définit des formules partagées pour une plage de cellules.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formule partagée. |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Définit une formule pour une plage de cellules.

**Remarks**

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Cette propriété sera supprimée 12 mois plus tard depuis décembre 2019. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formule partagée. |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| isR1C1 | boolean | si la formule est une formule R1C1 |
| isLocal | boolean | si la formule est formatée selon la locale |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Définit des formules partagées pour une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formule partagée. |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Définit des formules partagées pour une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formule partagée. |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options pour analyser la formule. |
| valeurs | java.lang.Object[][] | valeurs pour ces cellules avec la formule partagée donnée |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Définit le style de la cellule.

**Remarks**

Si les paramètres de bordure sont modifiés, la bordure des cellules d'ajustement sera également mise à jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Le style de cellule. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Appliquer la propriété modifiée du style à la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Le style de cellule. |
| explicitFlag | boolean | Vrai, uniquement en écrasant le formatage qui est explicitement défini. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Appliquer le style de la cellule en fonction des indicateurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Le style de cellule. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Le drapeau de style. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Créer un tableau de données à une variable pour la plage donnée à partir de cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| rowIndexOfInputCell | int | indice de ligne de la cellule d'entrée |
| columnIndexOfInputCell | int | indice de colonne de la cellule d'entrée |
| isRowInput | boolean | Indique si la cellule d'entrée est une cellule d'entrée de ligne (true) ou une cellule d'entrée de colonne (false). |
| valeurs | java.lang.Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Créer un tableau de données à deux variables pour la plage donnée à partir de cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| rowIndexOfRowInputCell | int | indice de ligne de la cellule d'entrée de ligne |
| columnIndexOfRowInputCell | int | indice de colonne de la cellule d'entrée de ligne |
| rowIndexOfColumnInputCell | int | indice de ligne de la cellule d'entrée de colonne |
| columnIndexOfColumnInputCell | int | indice de colonne de la cellule d'entrée de colonne |
| valeurs | java.lang.Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Créer un tableau de données à une variable pour la plage donnée à partir de cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| inputCell | java.lang.String | la cellule d'entrée |
| isRowInput | boolean | Indique si la cellule d'entrée est une cellule d'entrée de ligne (true) ou une cellule d'entrée de colonne (false). |
| valeurs | java.lang.Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Créer un tableau de données à deux variables pour la plage donnée à partir de cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowNumber | int | Nombre de lignes à remplir dans la formule. |
| columnNumber | int | Nombre de colonnes à remplir dans la formule. |
| rowInputCell | java.lang.String | la cellule d'entrée de ligne |
| columnInputCell | java.lang.String | la cellule d'entrée de colonne |
| valeurs | java.lang.Object[][] | valeurs pour les cellules dans la plage de formule du tableau |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Définit la valeur contenue dans cette cellule.

**Remarks**

Type possible :

null,

Boolean,

DateTime,

Double,

Integer

String.

Pour une valeur int, elle peut être renvoyée sous forme d'un objet Integer ou d'un objet Double. Et il n'y a aucune garantie que la valeur renvoyée reste toujours du même type d'objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Convertir la [Cell](../../com.aspose.cells/cell) en données de structure JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'objet Cell actuel.

**Returns:**
java.lang.String -
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


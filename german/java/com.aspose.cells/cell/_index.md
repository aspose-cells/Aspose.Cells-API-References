---
title: "Zelle"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das eine einzelne Arbeitsmappenzelle repräsentiert."
type: docs
url: /de/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Kapselt das Objekt, das eine einzelne Arbeitsmappenzelle repräsentiert.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Berechnet die Formel der Zelle. |
| [characters(int startIndex, int length)](#characters-int-int-) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Zellentext darstellt. |
| [containsExternalLink()](#containsExternalLink--) | Gibt an, ob diese Zelle einen externen Link enthält. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Kopiert Daten aus einer Quellzelle. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes Zellenobjekt bezieht. |
| [equals(Object obj)](#equals-java.lang.Object-) | Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes bezieht. |
| [getArrayRange()](#getArrayRange--) | Ermittelt den Arraybereich, wenn die Formel der Zelle eine Array-Formel ist. |
| [getBoolValue()](#getBoolValue--) | Ermittelt den booleschen Wert, der in der Zelle enthalten ist. |
| [getCharacters()](#getCharacters--) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zellentext darstellen. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zellentext darstellen. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ermittelt die Spaltennummer (nullbasiert) der Zelle. |
| [getComment()](#getComment--) | Ermittelt den Kommentar dieser Zelle. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Ermittelt das Ergebnis der bedingten Formatierung. |
| [getDateTimeValue()](#getDateTimeValue--) | Ermittelt den DateTime-Wert, der in der Zelle enthalten ist. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Ermittelt alle Zellen, deren Formel direkt auf diese Zelle verweist. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Ermittelt alle Zellen, deren berechnetes Ergebnis von dieser Zelle abhängt. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Ermittelt den formatierten Zeichenkettenwert dieser Zelle anhand des Anzeigestils der Zelle. |
| [getDisplayStyle()](#getDisplayStyle--) | Ermittelt den Anzeigestil dieser Zelle. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Ermittelt den Anzeigestil dieser Zelle. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Ermittelt den Anzeigestil dieser Zelle. |
| [getDoubleValue()](#getDoubleValue--) | Ermittelt den Double-Wert, der in der Zelle enthalten ist. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Ermittelt das eingebettete Bild in der Zelle. |
| [getFloatValue()](#getFloatValue--) | Ermittelt den Float-Wert, der in der Zelle enthalten ist. |
| [getFormatConditions()](#getFormatConditions--) | Ermittelt Formatbedingungen, die auf diese Zelle angewendet werden. |
| [getFormula()](#getFormula--) | Ermittelt eine Formel der [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Ermittelt die Formel dieser Zelle. |
| [getFormulaLocal()](#getFormulaLocal--) | Ermittelt die lokalisierte formatierte Formel der Zelle. |
| [getHeightOfValue()](#getHeightOfValue--) | Ermittelt die Höhe des Werts in Pixeln. |
| [getHtmlString()](#getHtmlString--) | Ermittelt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Ermittelt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [getIntValue()](#getIntValue--) | Ermittelt den Integer-Wert, der in der Zelle enthalten ist. |
| [getLeafs()](#getLeafs--) | Alle Zellen abrufen, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Alle Zellen abrufen, die aktualisiert werden, wenn diese Zelle geändert wird. |
| [getMergedRange()](#getMergedRange--) | Gibt ein [Bereich](../../com.aspose.cells/range)-Objekt zurück, das einen zusammengeführten Bereich darstellt. |
| [getName()](#getName--) | Liefert den Namen der Zelle. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Stellt den Kategorie‑Typ der Zahlenformatierung dieser Zelle dar. |
| [getPicture()](#getPicture--) | Ruft eine [Bild](../../com.aspose.cells/picture)-Instanz ab, die das eingebettete Bild in dieser Zelle darstellt, oder null, wenn für diese Zelle kein eingebettetes Bild vorhanden ist. |
| [getPrecedents()](#getPrecedents--) | Ruft alle Verweise ab, die in der Formel dieser Zelle vorkommen. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Ruft alle Vorgänger (Verweise auf Zellen in der aktuellen Arbeitsmappe) ab, die von der Formel dieser Zelle bei deren Berechnung verwendet werden. |
| [getR1C1Formula()](#getR1C1Formula--) | Ruft eine R1C1‑Formel der [Zelle](../../com.aspose.cells/cell) ab. |
| [getRichValue()](#getRichValue--) | Ruft den Rich‑Wert der Zelle ab. |
| [getRow()](#getRow--) | Ruft die Zeilennummer (nullbasiert) der Zelle ab. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Ruft den gemeinsam genutzten Stilindex der Zelle im Stilpool ab. |
| [getStringValue()](#getStringValue--) | Ruft den Zeichenkettenwert ab, der in der Zelle enthalten ist. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Ruft den Zeichenkettenwert nach einer bestimmten Formatierungsstrategie ab. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Ruft den Wert der Zelle als Zeichenkette ohne Formatierung ab. |
| [getStyle()](#getStyle--) | Ruft den Zellenstil ab. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Wenn checkBorders wahr ist, prüfen, ob die Ränder anderer Zellen den Stil dieser Zelle beeinflussen. |
| [getTable()](#getTable--) | Ruft die Tabelle ab, die diese Zelle enthält. |
| [getType()](#getType--) | Stellt den Zellenwerttyp dar. |
| [getValidation()](#getValidation--) | Ruft die auf diese Zelle angewendete Validierung ab. |
| [getValidationValue()](#getValidationValue--) | Ruft den Wert der auf diese Zelle angewendeten Validierung ab. |
| [getValue()](#getValue--) | Ruft den in dieser Zelle enthaltenen Wert ab. |
| [getWidthOfValue()](#getWidthOfValue--) | Ruft die Breite des Wertes in Pixeln ab. |
| [getWorksheet()](#getWorksheet--) | Ruft das übergeordnete Arbeitsblatt ab. |
| [hasCustomFunction()](#hasCustomFunction--) | Prüft, ob in der Formel dieser Zelle eine benutzerdefinierte Funktion (nicht unterstützte Funktion) vorhanden ist. |
| [hasCustomStyle()](#hasCustomStyle--) | Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen (anders als die standardmäßig von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbten) hat. |
| [hashCode()](#hashCode--) | Dient als Hash-Funktion für einen bestimmten Typ. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Fügen Sie einige Zeichen in die Zelle ein. |
| [isArrayFormula()](#isArrayFormula--) | Gibt an, ob die Zellformel eine Array-Formel ist. |
| [isArrayHeader()](#isArrayHeader--) | Gibt an, dass die Zellformel eine Array-Formel ist und dass sie die erste Zelle des Arrays ist. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Gibt an, ob die Zellformel eine dynamische Array-Formel (true) oder eine Legacy-Array-Formel (false) ist. |
| [isErrorValue()](#isErrorValue--) | Prüft, ob der Wert dieser Zelle ein Fehler ist. |
| [isFormula()](#isFormula--) | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [isInArray()](#isInArray--) | Gibt an, ob die Zellformel eine Array-Formel ist. |
| [isInTable()](#isInTable--) | Gibt an, ob diese Zelle Teil einer Tabellenformel ist. |
| [isMerged()](#isMerged--) | Prüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht. |
| [isNumericValue()](#isNumericValue--) | Gibt an, ob der Wert dieser Zelle numerisch ist (int, double und datetime). |
| [isRichText()](#isRichText--) | Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist. |
| [isSharedFormula()](#isSharedFormula--) | Gibt an, ob die Zellformel Teil einer gemeinsamen Formel ist. |
| [isStyleSet()](#isStyleSet--) | Gibt an, ob der Stil der Zelle festgelegt ist. |
| [isTableFormula()](#isTableFormula--) | Gibt an, ob diese Zelle Teil einer Tabellenformel ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Schreibt einen booleschen Wert in die Zelle. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Schreibt einen DateTime-Wert in die Zelle. |
| [putValue(double doubleValue)](#putValue-double-) | Schreibt einen double-Wert in die Zelle. |
| [putValue(int intValue)](#putValue-int-) | Schreibt einen ganzzahligen Wert in die Zelle. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Schreibt einen Objektwert in die Zelle. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Schreibt einen Zeichenkettenwert in die Zelle. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Schreibt einen Zeichenkettenwert in die Zelle und konvertiert den Wert bei Bedarf in einen anderen Datentyp. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Schreibt einen Wert in die Zelle; bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Array-Formel entfernen. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Text der Zelle mit Optionen ersetzen. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Setzt eine Array-Formel (Legacy-Array-Formel, die in MS Excel über STRG+UMSCHALT+EINGABE eingegeben wird) für einen Zellbereich. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Setzt eine Array-Formel für einen Zellbereich. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Setzt eine Array-Formel für einen Zellbereich. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Setzt eine Array-Formel für einen Zellbereich. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Setzt das Rich-Text-Format der Zelle. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Setzt das eingebettete Bild in der Zelle. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Setzt eine Formel des [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Setze die Formel und den Wert der Formel. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Setze die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Setze die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Setze die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Ermittelt die lokalisierte formatierte Formel der Zelle. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Setzt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Setzt eine R1C1-Formel des [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Setzt eine Formel für einen Zellbereich. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Setzt den Zellenstil. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Wendet die geänderte Eigenschaft des Stils auf die Zelle an. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet den Zellenstil basierend auf Flags an. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Erstelle eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Erstelle eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Erstelle eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Erstelle eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Setzt den in dieser Zelle enthaltenen Wert. |
| [toJson()](#toJson--) | Konvertiere [Cell](../../com.aspose.cells/cell) in JSON-Strukturdaten. |
| [toString()](#toString--) | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Berechnet die Formel der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen für die Berechnung |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Zellentext darstellt.

**Remarks**

Diese Methode funktioniert nur bei Zellen mit Zeichenkettenwert.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Index des Beginns des Zeichens. |
| length | int | Die Anzahl der Zeichen. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Kopiert Daten aus einer Quellzelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Quell-[Cell](../../com.aspose.cells/cell)-Objekt. |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes Zellenobjekt bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | ein weiteres Zellenobjekt |

**Returns:**
boolean - true, wenn zwei Zellenobjekte auf dieselbe Zelle verweisen.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | ein weiteres Objekt |

**Returns:**
boolean - true, wenn zwei Objekte auf dieselbe Zelle verweisen.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Ermittelt den Arraybereich, wenn die Formel der Zelle eine Array-Formel ist.

**Remarks**

Gilt nur, wenn die Formel der Zelle eine Array-Formel ist.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Ermittelt den booleschen Wert, der in der Zelle enthalten ist.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zellentext darstellen.

**Returns:**
com.aspose.cells.FontSetting[] - Alle Characters objects
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Zellentext darstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Flag | boolean | Gibt an, ob ein Tabellenstil auf die Zelle angewendet wird, wenn die Zelle in der Tabelle ist. |

**Returns:**
com.aspose.cells.FontSetting[] - Alle Characters objects
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


Ermittelt die Spaltennummer (nullbasiert) der Zelle.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Ermittelt den Kommentar dieser Zelle.

**Remarks**

Wenn kein Kommentar auf die Zelle zutrifft, wird null zurückgegeben.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Ermittelt das Ergebnis der bedingten Formatierung.

**Remarks**

Gibt null zurück, wenn auf diese Zelle keine bedingte Formatierung angewendet wird,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Ermittelt den DateTime-Wert, der in der Zelle enthalten ist.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Ermittelt alle Zellen, deren Formel direkt auf diese Zelle verweist.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAll | boolean | Gibt an, ob Formeln in anderen Arbeitsblättern geprüft werden sollen |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Ermittelt alle Zellen, deren berechnetes Ergebnis von dieser Zelle abhängt.

**Remarks**

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass das Arbeitsbuch für [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) auf den Wert true gesetzt wurde und mit dieser Einstellung vollständig berechnet ist. Wenn es keinen Formelbezug zu dieser Zelle gibt, wird null zurückgegeben.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rekursiv | boolean | Ob diejenigen Abhängigen zurückgegeben werden, die nicht direkt auf diese Zelle verweisen, sondern auf andere Blätter dieser Zelle. |

**Returns:**
java.util.Iterator - Aufzählung, um alle abhängigen (Zellobjekte) zu enumerieren
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Ermittelt den formatierten Zeichenkettenwert dieser Zelle anhand des Anzeigestils der Zelle.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Ermittelt den Anzeigestil dieser Zelle.

**Remarks**

Entspricht der Verwendung von [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) für [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). Das heißt, diese Methode prüft und passt die oberen/unteren/linken/rechten Rahmen dieser Zelle gemäß dem Stil ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) ihrer benachbarten Zellen an, prüft jedoch nicht die zusammengeführten Zellen und nicht den Anzeigestil der benachbarten Zellen.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Ermittelt den Anzeigestil dieser Zelle.

**Remarks**

Wenn das angegebene Flag false ist, entspricht es [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). Andernfalls entspricht es der Verwendung von [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) für [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| includeMergedBorders | boolean | Gibt an, ob die Rahmen zusammengeführter Zellen geprüft werden. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Ermittelt den Anzeigestil dieser Zelle.

**Remarks**

Wenn diese Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listobjekten usw. betroffen ist, kann der Anzeigestil von [getStyle()](../../com.aspose.cells/cell\#getStyle--) abweichen.

Bei Flags zur Anpassung von Rahmen an benachbarte Zellen geben [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) an, ob die unteren/oberen/rechten/linken Rahmen der links/rechts/oben/unten benachbarten Zellen geprüft und kombiniert werden.

Aus Leistungs- und Kompatibilitätsgründen werden einige Enums verwendet, um besondere Vorgänge zu kennzeichnen:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Bitte beachten Sie, dass das Überprüfen von Rändern/Styles benachbarter Zellen, insbesondere der Anzeigestile, ein zeitaufwändiger Vorgang ist. Wenn es nicht nötig ist, die Ränder für den zurückgegebenen Stil zu ermitteln, führt die Verwendung von [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) zum Deaktivieren des Prozesses für benachbarte Zellen zu besserer Leistung. Beim Abrufen der Ränder benachbarter Zellen aus nur auf diesen Zellen definierten Stilen (ohne Einstellung von [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)) kann die Leistung ebenfalls besser sein, da das Prüfen des Anzeigestils einer Zelle ebenfalls zeitaufwändig ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Gibt an, welche Ränder überprüft und gemäß den Rändern benachbarter Zellen angepasst werden müssen. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Ermittelt den Double-Wert, der in der Zelle enthalten ist.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Ermittelt das eingebettete Bild in der Zelle.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Ermittelt den Float-Wert, der in der Zelle enthalten ist.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Ermittelt Formatbedingungen, die auf diese Zelle angewendet werden.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Gibt ein [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection) Objekt zurück
### getFormula() {#getFormula--}
```
public String getFormula()
```


Ermittelt eine Formel der [Cell](../../com.aspose.cells/cell).

**Remarks**

Eine Formelzeichenkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte verwenden Sie stets das Komma (,) als Parametertrennzeichen, zum Beispiel "=SUM(A1, E1, H2)".

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


Ermittelt die Formel dieser Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - die Formel dieser Zelle.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Ermittelt die lokalisierte formatierte Formel der Zelle.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Ermittelt die Höhe des Werts in Pixeln.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Ermittelt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Ermittelt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| html5 | boolean | Gibt an, ob der Wert mit html5 kompatibel ist |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Ermittelt den Integer-Wert, der in der Zelle enthalten ist.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Alle Zellen abrufen, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.GetDependentsInCalculation(bool), um alle Abhängigkeiten in der Berechnungskette zu erhalten. Diese Eigenschaft wird 12 Monate nach Mai 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

**Returns:**
java.util.Iterator - Aufzählung zur Enumeration aller Abhängigkeiten (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Alle Zellen abrufen, die aktualisiert werden, wenn diese Zelle geändert wird.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.GetDependentsInCalculation(bool), um alle Abhängigkeiten in der Berechnungskette zu erhalten. Diese Eigenschaft wird 12 Monate nach Mai 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rekursiv | boolean | Ob Blätter zurückgegeben werden, die nicht direkt auf diese Zelle verweisen, sondern auf andere Blätter dieser Zelle |

**Returns:**
java.util.Iterator - Aufzählung zur Enumeration aller Abhängigkeiten (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Gibt ein [Bereich](../../com.aspose.cells/range)-Objekt zurück, das einen zusammengeführten Bereich darstellt.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen der Zelle.

**Remarks**

Ein Zellenname enthält den Spaltenbuchstaben und die Zeilennummer. Zum Beispiel ist der Name einer Zelle in Zeile 0 und Spalte 0 A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Stellt den Kategorie‑Typ der Zahlenformatierung dieser Zelle dar.

Siehe [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Wenn das Formatierungsmuster einer Zelle mit bedingten Formatierungsmustern kombiniert wird, entspricht der zurückgegebene Typ dem Teil, der für den aktuellen Wert dieser Zelle verwendet wird. Zum Beispiel, wenn das Formatierungsmuster für diese Zelle "\#,\#\#0;(\#,\#\#0);"-";@" ist, dann ist, wenn der Zellenwert numerisch und nicht 0 ist, der zurückgegebene Typ [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER); Wenn der Zellenwert 0 oder kein numerischer Wert ist, ist der zurückgegebene Typ [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Ruft eine [Bild](../../com.aspose.cells/picture)-Instanz ab, die das eingebettete Bild in dieser Zelle darstellt, oder null, wenn für diese Zelle kein eingebettetes Bild vorhanden ist.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Ruft alle Verweise ab, die in der Formel dieser Zelle vorkommen.

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


Ruft alle Vorgänger (Verweise auf Zellen in der aktuellen Arbeitsmappe) ab, die von der Formel dieser Zelle bei deren Berechnung verwendet werden.

**Remarks**

Diese Methode funktioniert nur, wenn [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) für die Arbeitsmappe true ist und die Arbeitsmappe vollständig berechnet wurde. Wenn diese Zelle keine Formel ist oder nicht auf andere Zellen verweist, wird null zurückgegeben.

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
java.util.Iterator - Aufzählung zur Enumeration aller Referenzen (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Ruft eine R1C1‑Formel der [Zelle](../../com.aspose.cells/cell) ab.

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Ruft den Rich‑Wert der Zelle ab.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Ruft die Zeilennummer (nullbasiert) der Zelle ab.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Ruft den gemeinsam genutzten Stilindex der Zelle im Stilpool ab.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Liefert den Zeichenkettenwert, der in der Zelle enthalten ist. Wenn der Typ dieser Zelle Zeichenkette ist, wird der Zeichenkettenwert selbst zurückgegeben. Für andere Zellentypen wird der formatierte Zeichenkettenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben. Der formatierte Zellenwert ist derselbe wie das, was Sie aus Excel erhalten, wenn Sie eine Zelle als Text kopieren (z. B. das Kopieren der Zelle in einen Texteditor oder das Exportieren in CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Ruft den Zeichenkettenwert nach einer bestimmten Formatierungsstrategie ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). Die formatierte Strategie. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Ruft den Wert der Zelle als Zeichenkette ohne Formatierung ab.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Stattdessen sollte der Benutzer das Werteobjekt abrufen und es gemäß dem Werttyp und den spezifischen Anforderungen formatieren. Diese Eigenschaft wird 12 Monate später, seit Dezember 2020, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ruft den Zellenstil ab.

**Remarks**

Um den Stil der Zelle zu ändern, rufen Sie bitte die Methode Cell.SetStyle() auf, nachdem Sie das zurückgegebene Stilobjekt geändert haben. Diese Methode ist identisch mit [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) mit dem Wert true für den Parameter.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Wenn checkBorders wahr ist, prüfen, ob die Ränder anderer Zellen den Stil dieser Zelle beeinflussen.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| checkBorders | boolean | Prüfen Sie die Ränder anderer Zellen |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Ruft die Tabelle ab, die diese Zelle enthält.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Stellt den Zellenwerttyp dar.

Siehe [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Ruft die auf diese Zelle angewendete Validierung ab.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Ruft den Wert der auf diese Zelle angewendeten Validierung ab.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Ruft den in dieser Zelle enthaltenen Wert ab.

**Remarks**

Möglicher Typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

Für int-Werte kann er als Integer-Objekt oder als Double-Objekt zurückgegeben werden. Und es gibt keine Garantie, dass der zurückgegebene Wert stets als derselbe Objekttyp beibehalten wird.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Ruft die Breite des Wertes in Pixeln ab.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ruft das übergeordnete Arbeitsblatt ab.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Prüft, ob in der Formel dieser Zelle eine benutzerdefinierte Funktion (nicht unterstützte Funktion) vorhanden ist.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen (anders als die standardmäßig von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbten) hat.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hash-Funktion für einen bestimmten Typ.

**Returns:**
int – Ein Hashcode für das aktuelle Cell-Objekt.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Fügen Sie einige Zeichen in die Zelle ein. Wenn die Zelle reich formatiert ist, kann diese Methode die ursprüngliche Formatierung beibehalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |
| Text | java.lang.String | Eingefügter Text. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Gibt an, ob die Zellformel eine Array-Formel ist.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Gibt an, dass die Zellformel eine Array-Formel ist und dass sie die erste Zelle des Arrays ist.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Gibt an, ob die Zellformel eine dynamische Array-Formel (true) oder eine Legacy-Array-Formel (false) ist.

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Prüft, ob der Wert dieser Zelle ein Fehler ist.

**Remarks**

Gilt auch für Formelfelder, um zu prüfen, ob das berechnete Ergebnis ein Fehler ist.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Gibt an, ob die angegebene Zelle eine Formel enthält.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Gibt an, ob die Zellformel eine Array-Formel ist.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen bitte Cell.IsArrayFormula, um zu prüfen, ob die Zellformel eine Array-Formel ist. Diese Eigenschaft wird 12 Monate später, seit Mai 2018, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Gibt an, ob diese Zelle Teil einer Tabellenformel ist.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen bitte Cell.IsTableFormula, um zu prüfen, ob die Zellformel Teil einer Tabellenformel ist. Diese Eigenschaft wird 12 Monate später, seit Mai 2018, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Prüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Gibt an, ob der Wert dieser Zelle numerisch ist (int, double und datetime).

**Remarks**

Gilt auch für Formelfelder, um das berechnete Ergebnis zu prüfen

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Gibt an, ob die Zellformel Teil einer gemeinsamen Formel ist.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Gibt an, ob der Stil der Zelle gesetzt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Gibt an, ob diese Zelle Teil einer Tabellenformel ist.

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


Schreibt einen booleschen Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Schreibt einen DateTime-Wert in die Zelle.

**Remarks**

Das Festlegen eines DateTime-Werts für eine Zelle bedeutet nicht, dass die Zelle automatisch als Datum/Uhrzeit formatiert wird. Der DateTime-Wert wird im Datenmodell von sowohl MS Excel als auch Aspose.Cells als numerischer Wert gespeichert. Ob der numerische Wert als solcher oder als Datum/Uhrzeit interpretiert wird, hängt vom auf diese Zelle angewendeten Zahlenformat ab. Wenn diese Zelle nicht als Datum/Uhrzeit formatiert ist, wird sie als numerischer Wert angezeigt, obwohl Sie einen DateTime eingegeben haben.

**Example**

Dieses Beispiel zeigt, wie man einen DateTime-Wert in einer Zelle festlegt und ihn als Datum/Uhrzeit anzeigen lässt.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Eingabewert |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Schreibt einen double-Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleValue | double | Eingabewert |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Schreibt einen ganzzahligen Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intValue | int | Eingabewert |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Schreibt einen Objektwert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objectValue | java.lang.Object | Eingabewert |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Schreibt einen Zeichenkettenwert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Schreibt einen Zeichenkettenwert in die Zelle und konvertiert den Wert bei Bedarf in einen anderen Datentyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Schreibt einen Wert in die Zelle; bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Array-Formel entfernen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| leaveNormalFormula | boolean | True steht für die Umwandlung der Array-Formel in eine normale Formel. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Text der Zelle mit Optionen ersetzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValue | java.lang.String | String-Wert zum Ersetzen |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Die Ersetzungsoptionen |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Setzt eine Array-Formel (Legacy-Array-Formel, die in MS Excel über STRG+UMSCHALT+EINGABE eingegeben wird) für einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array-Formel. |
| rowNumber | int | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | int | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Setzt eine Array-Formel für einen Zellbereich.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Diese Eigenschaft wird 12 Monate nach Dezember 2019 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array-Formel. |
| rowNumber | int | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | int | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| isR1C1 | boolean | ob die Formel eine R1C1-Formel ist |
| isLocal | boolean | ob die Formel lokalisierungsformatiert ist |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Setzt eine Array-Formel für einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array-Formel. |
| rowNumber | int | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | int | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Setzt eine Array-Formel für einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array-Formel. |
| rowNumber | int | Anzahl der Zeilen, um das Ergebnis der Array-Formel zu füllen. |
| columnNumber | int | Anzahl der Spalten, um das Ergebnis der Array-Formel zu füllen. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |
| Werte | java.lang.Object[][] | Werte für jene Zellen mit gegebener Array-Formel |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Setzt das Rich-Text-Format der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Alle Characters-Objekte. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen.

**Remarks**

Der zurückgegebene Bereich stimmt möglicherweise nicht mit dem tatsächlichen Bereich überein, in den diese dynamische Array-Formel ausläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit "\\#SPILL!" markiert. In einer solchen Situation geben wir jedoch weiterhin den gesamten Bereich zurück, in den diese Formel auslaufen sollte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | der Formelausdruck |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. Die "Parse"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| calculateValue | boolean | ob diese dynamische Array-Formel für diese Zellen im ausgegebenen Bereich berechnet wird. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen.

**Remarks**

Der zurückgegebene Bereich stimmt möglicherweise nicht mit dem tatsächlichen Bereich überein, in den diese dynamische Array-Formel ausläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit "\\#SPILL!" markiert. In einer solchen Situation geben wir jedoch weiterhin den gesamten Bereich zurück, in den diese Formel auslaufen sollte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | der Formelausdruck |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. Die "Parse"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| Werte | java.lang.Object[][] | Werte(berechnete Ergebnisse) für diese Zellen mit gegebener dynamischer Array-Formel |
| calculateRange | boolean | Ob der ausgegebene Bereich für diese dynamische Array-Formel berechnet wird. Wenn der Parameter "values" nicht null ist und dieses Flag false ist, dann ist die Höhe des ausgegebenen Bereichs values.Length und die Breite ist values[0].Length. |
| calculateValue | boolean | ob diese dynamische Array-Formel für diese Zellen im ausgegebenen Bereich berechnet wird, wenn "values" null ist oder das entsprechende Element in "values" für eine Zelle null ist. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Setzt eine dynamische Array-Formel und lässt die Formel, falls möglich, in benachbarte Zellen überlaufen.

**Remarks**

Der zurückgegebene Bereich stimmt möglicherweise nicht mit dem tatsächlichen Bereich überein, in den diese dynamische Array-Formel ausläuft. Wenn im Bereich nicht leere Zellen vorhanden sind, wird die Formel nur für die aktuelle Zelle gesetzt und mit "\\#SPILL!" markiert. In einer solchen Situation geben wir jedoch weiterhin den gesamten Bereich zurück, in den diese Formel auslaufen sollte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arrayFormula | java.lang.String | der Formelausdruck |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. Die "Parse"-Option wird ignoriert und die Formel wird immer sofort geparst. |
| Werte | java.lang.Object[][] | Werte(berechnete Ergebnisse) für diese Zellen mit gegebener dynamischer Array-Formel |
| calculateRange | boolean | Ob der ausgegebene Bereich für diese dynamische Array-Formel berechnet wird. Wenn der Parameter "values" nicht null ist und dieses Flag false ist, dann ist die Höhe des ausgegebenen Bereichs values.Length und die Breite ist values[0].Length. |
| calculateValue | boolean | ob diese dynamische Array-Formel für diese Zellen im ausgegebenen Bereich berechnet wird, wenn "values" null ist oder das entsprechende Element in "values" für eine Zelle null ist. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Die Optionen zur Berechnung der Formel. In der Regel sollte aus Leistungsgründen die Eigenschaft [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\\#getRecursive--) false sein. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Setzt das eingebettete Bild in der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Setzt eine Formel des [Cell](../../com.aspose.cells/cell).

**Remarks**

Eine Formelzeichenkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte verwenden Sie stets das Komma (,) als Parametertrennzeichen, zum Beispiel "=SUM(A1, E1, H2)".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Setze die Formel und den Wert der Formel.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetFormula(string,FormulaParseOptions,object). Diese Eigenschaft wird 12 Monate später, seit Dezember 2019, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die Formel. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |
| Wert | java.lang.Object | Der Wert der Formel. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Setze die Formel und den Wert (berechnetes Ergebnis) der Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die Formel. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Setze die Formel und den Wert (berechnetes Ergebnis) der Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die Formel. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |
| Wert | java.lang.Object | Der Wert(berechnetes Ergebnis) der Formel. |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Setze die Formel und den Wert (berechnetes Ergebnis) der Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die Formel. |
| Wert | java.lang.Object | Der Wert(berechnetes Ergebnis) der Formel. |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Ermittelt die lokalisierte formatierte Formel der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Setzt die HTML-Zeichenkette, die Daten und einige Formate in dieser Zelle enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Setzt eine R1C1-Formel des [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Setzt gemeinsam genutzte Formeln für einen Zellbereich.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | java.lang.String | Gemeinsame Formel. |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Setzt eine Formel für einen Zellbereich.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Diese Eigenschaft wird 12 Monate später, seit Dezember 2019, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | java.lang.String | Gemeinsame Formel. |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| isR1C1 | boolean | ob die Formel eine R1C1-Formel ist |
| isLocal | boolean | ob die Formel lokalisierungsformatiert ist |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Setzt gemeinsam genutzte Formeln für einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | java.lang.String | Gemeinsame Formel. |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Setzt gemeinsam genutzte Formeln für einen Zellbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sharedFormula | java.lang.String | Gemeinsame Formel. |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Optionen zum Parsen der Formel. |
| Werte | java.lang.Object[][] | Werte für diese Zellen mit gegebener gemeinsamer Formel |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Setzt den Zellenstil.

**Remarks**

Wenn die Rahmen-Einstellungen geändert werden, wird der Rahmen der angepassten Zellen ebenfalls aktualisiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Der Zellenstil. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Wendet die geänderte Eigenschaft des Stils auf die Zelle an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Der Zellenstil. |
| explicitFlag | boolean | True, überschreibt nur Formatierungen, die explizit festgelegt wurden. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Wendet den Zellenstil basierend auf Flags an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Der Zellenstil. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Das Stil-Flag. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Erstelle eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| rowIndexOfInputCell | int | Zeilenindex der Eingabezelle |
| columnIndexOfInputCell | int | Spaltenindex der Eingabezelle |
| isRowInput | boolean | Gibt an, ob die Eingabezelle eine Zeileneingabezelle (true) oder eine Spalteneingabezelle (false) ist. |
| Werte | java.lang.Object[][] | Werte für Zellen im Tabellenformelbereich |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Erstelle eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| rowIndexOfRowInputCell | int | Zeilenindex der Zeileneingabezelle |
| columnIndexOfRowInputCell | int | Spaltenindex der Zeileneingabezelle |
| rowIndexOfColumnInputCell | int | Zeilenindex der Spalteneingabezelle |
| columnIndexOfColumnInputCell | int | Spaltenindex der Spalteneingabezelle |
| Werte | java.lang.Object[][] | Werte für Zellen im Tabellenformelbereich |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Erstelle eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| inputCell | java.lang.String | die Eingabezelle |
| isRowInput | boolean | Gibt an, ob die Eingabezelle eine Zeileneingabezelle (true) oder eine Spalteneingabezelle (false) ist. |
| Werte | java.lang.Object[][] | Werte für Zellen im Tabellenformelbereich |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Erstelle eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | int | Anzahl der Zeilen, die die Formel ausfüllen sollen. |
| columnNumber | int | Anzahl der Spalten, die die Formel ausfüllen sollen. |
| rowInputCell | java.lang.String | die Zeileneingabezelle |
| columnInputCell | java.lang.String | die Spalteneingabezelle |
| Werte | java.lang.Object[][] | Werte für Zellen im Tabellenformelbereich |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Setzt den in dieser Zelle enthaltenen Wert.

**Remarks**

Möglicher Typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

Für int-Werte kann er als Integer-Objekt oder als Double-Objekt zurückgegeben werden. Und es gibt keine Garantie, dass der zurückgegebene Wert stets als derselbe Objekttyp beibehalten wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Konvertiere [Cell](../../com.aspose.cells/cell) in JSON-Strukturdaten.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


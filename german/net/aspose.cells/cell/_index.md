---
title: Cell
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das eine einzelne Workbook-Zelle darstellt.
type: docs
weight: 230
url: /de/net/aspose.cells/cell/
---
## Cell class

Kapselt das Objekt, das eine einzelne Workbook-Zelle darstellt.

```csharp
public class Cell
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Ruft den in der Zelle enthaltenen booleschen Wert ab. |
| [Column](../../aspose.cells/cell/column) { get; } | Ruft die Spaltennummer (nullbasiert) der Zelle ab. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Ruft den Kommentar dieser Zelle ab. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Ruft den in der Zelle enthaltenen DateTime-Wert ab. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Ruft den formatierten Zeichenfolgenwert dieser Zelle nach Anzeigestil der Zelle ab. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Ruft den in der Zelle enthaltenen Double-Wert ab. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Ruft den Float-Wert ab, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Ruft eine Formel von ab oder legt sie fest[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Holen Sie sich die gebietsschemaformatierte Formel der Zelle. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formate in dieser Zelle enthält. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Ruft den in der Zelle enthaltenen ganzzahligen Wert ab. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Gibt an, ob die Zellenformel eine Matrixformel ist. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Gibt an, dass die Formel der Zelle und die Array-Formel ist und es sich um die erste Zelle des Arrays handelt. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Überprüft, ob der Wert dieser Zelle ein Fehler ist. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Stellt dar, ob die angegebene Zelle eine Formel enthält. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Überprüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Gibt an, ob der innere Wert dieser Zelle numerisch ist (int, double und datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Gibt an, ob die Zellformel Teil einer freigegebenen Formel ist. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Gibt an, ob der Stil der Zelle eingestellt ist. Wenn "false" zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Gibt an, ob diese Zelle Teil der Tabellenformel ist. |
| [Name](../../aspose.cells/cell/name) { get; } | Ruft den Namen der Zelle ab. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Repräsentiert den Kategorietyp der Zahlenformatierung dieser Zelle. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Ruft eine R1C1-Formel ab oder legt sie fest[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Ruft die Zeilennummer (nullbasiert) der Zelle ab. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Ruft den gemeinsam genutzten Stilindex der Zelle im Stilpool ab. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Ruft den in der Zelle enthaltenen Zeichenfolgenwert ab. Wenn der Typ dieser Zelle eine Zeichenfolge ist, geben Sie den Zeichenfolgenwert selbst zurück. Für andere Zelltypen wird der formatierte Zeichenfolgenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben. Der formatierte Zellenwert ist derselbe wie der von Ihnen kann aus Excel kommen, wenn eine Zelle als Text kopiert wird (z. B. Zelle in Texteditor kopieren oder in CSV exportieren). |
| [Type](../../aspose.cells/cell/type) { get; } | Repräsentiert den Zellwerttyp. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Ruft den in dieser Zelle enthaltenen Wert ab. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Ruft das übergeordnete Arbeitsblatt ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Berechnet die Formel der Zelle. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Gibt ein Characters-Objekt zurück, das einen Bereich von Zeichen im Zellentext darstellt. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Kopiert Daten aus einer Quellzelle. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Prüft, ob dieses Objekt auf dieselbe Zelle mit einem anderen Zellobjekt verweist. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Prüft, ob dieses Objekt mit einem anderen auf dieselbe Zelle verweist. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Ruft den Matrixbereich ab, wenn die Formel der Zelle eine Matrixformel ist. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Gibt alle Characters-Objekte zurück, die einen Bereich von Zeichen im Zellentext darstellen. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Gibt alle Characters-Objekte zurück, die einen Bereich von Zeichen im Zellentext darstellen. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Holen Sie sich das Ergebnis der bedingten Formatierung. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Alle Zellen abrufen, deren Formel direkt auf diese Zelle verweist. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Ruft alle Zellen ab, deren berechnetes Ergebnis von dieser Zelle abhängt. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Ruft den Anzeigestil der Zelle ab. Wenn diese Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listenobjekten usw. beeinflusst wird, dann kann der Anzeigestil von cell.GetStyle() abweichen. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Ruft den Anzeigestil der Zelle ab. Wenn die Zelle bedingt formatiert ist, ist der Anzeigestil nicht derselbe wie der von cell.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Ruft Formatbedingungen ab, die für diese Zelle gelten. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Holen Sie sich die Formel dieser Zelle. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Dient als Hash-Funktion für einen bestimmten Typ. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Ruft die Höhe des Werts in Pixeleinheiten ab. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Ruft die HTML-Zeichenfolge ab, die Daten und einige Formate in dieser Zelle enthält. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Gibt a zurück[`Range`](../range) Objekt, das einen zusammengeführten Bereich darstellt. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Ruft alle Referenzen ab, die in der Formel dieser Zelle vorkommen. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Ruft alle Präzedenzfälle (Verweis auf Zellen in der aktuellen Arbeitsmappe) ab, die von der Formel dieser Zelle verwendet werden, während sie berechnet wird. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Ruft den Zeichenfolgenwert durch eine bestimmte formatierte Strategie ab. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Ruft den Zellenstil ab. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Wenn checkBorders wahr ist, prüfen Sie, ob die Rahmen anderer Zellen den Stil dieser Zelle beeinflussen. |
| [GetTable](../../aspose.cells/cell/gettable)() | Ruft die Tabelle ab, die diese Zelle enthält. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Ruft die auf diese Zelle angewendete Validierung ab. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Ruft den Validierungswert ab, der auf diese Zelle angewendet wurde. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Ruft die Breite des Werts in Pixeleinheiten ab. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Gibt an, ob der Wert der Zellzeichenfolge ein Rich-Text ist. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Fügt einen booleschen Wert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Fügt einen DateTime-Wert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Fügt einen doppelten Wert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Fügt einen ganzzahligen Wert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Fügt einen Objektwert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Fügt einen Zeichenfolgenwert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Fügt einen Zeichenfolgenwert in die Zelle ein und konvertiert den Wert gegebenenfalls in einen anderen Datentyp. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Matrixformel entfernen. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Legt eine Array-Formel (alte Array-Formel, die über STRG+UMSCHALT+EINGABETASTE in MS Excel eingegeben wurde) auf einen Bereich von Zellen fest. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Legt eine Matrixformel auf einen Bereich von Zellen fest. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Legt eine Matrixformel auf einen Bereich von Zellen fest. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Legt das Rich-Text-Format der Zelle fest. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Stellen Sie die Formel und den Wert der Formel ein. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Stellen Sie die Formel und den Wert der Formel ein. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Setzt eine Formel auf einen Zellbereich. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Setzt eine Formel auf einen Zellbereich. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Setzt eine Formel auf einen Zellbereich. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Legt den Zellenstil fest. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Zellenstil anwenden. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Zellenstil anwenden. |
| override [ToString](../../aspose.cells/cell/tostring)() | Gibt eine Zeichenfolge zurück, die das aktuelle Cell-Objekt darstellt. |

### Beispiele

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Füge einen String in eine Zelle ein
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
//Gib eine ganze Zahl in eine Zelle
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

// Setzen Sie ein Double in eine Zelle
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//Füge eine Formel in eine Zelle ein
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Setze eine kombinierte Formel: "sum(average(b1,c1), b1)" in die Zelle bei b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

// Stil einer Zelle festlegen
Style style = cell.GetStyle();
//Hintergrundfarbe festlegen
style.BackgroundColor = Color.Yellow;
//Format einer Zelle festlegen
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Fügen Sie eine Zeichenfolge in eine Zelle ein
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
//Gib eine ganze Zahl in eine Zelle
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

// Setzen Sie ein Double in eine Zelle
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//Füge eine Formel in eine Zelle ein
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Setze eine kombinierte Formel: "sum(average(b1,c1), b1)" in die Zelle bei b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
// Stil einer Zelle festlegen
Dim style as Style = cell.GetStyle()

//Hintergrundfarbe festlegen
style.BackgroundColor = Color.Yellow
//Schriftart einer Zelle festlegen
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

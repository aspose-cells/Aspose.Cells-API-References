---
title: "Klasse Cell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Cell class. Kapselt das Objekt, das eine einzelne Arbeitsmappenzelle darstellt."
type: docs
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
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Liefert den booleschen Wert, der in der Zelle enthalten ist. |
| [Column](../../aspose.cells/cell/column/) { get; } | Liefert die Spaltennummer (nullbasiert) der Zelle. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Liefert den Kommentar dieser Zelle. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Liefert den DateTime-Wert, der in der Zelle enthalten ist. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Liefert den formatierten Zeichenkettenwert dieser Zelle gemäß dem Anzeigeformat der Zelle. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Liefert den double-Wert, der in der Zelle enthalten ist. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Liefert und setzt das eingebettete Bild in der Zelle. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Liefert den float-Wert, der in der Zelle enthalten ist. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Liefert oder setzt eine Formel des `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Liefert die lokalisierte formatierte Formel der Zelle. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Überprüft, ob es eine benutzerdefinierte Funktion (nicht unterstützte Funktion) in der Formel dieser Zelle gibt. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen hat (anders als die Standard‑Einstellungen, die von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbt werden). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Liefert und setzt die HTML‑Zeichenkette, die Daten und einige Formate in dieser Zelle enthält. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Liefert den ganzzahligen Wert, der in der Zelle enthalten ist. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Gibt an, ob die Zellenformel eine Array‑Formel ist. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Gibt an, dass die Formel der Zelle eine Array‑Formel ist und dass sie die erste Zelle des Arrays ist. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Gibt an, ob die Formel der Zelle eine dynamische Array‑Formel (true) oder eine Legacy‑Array‑Formel (false) ist. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Überprüft, ob der Wert dieser Zelle ein Fehler ist. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Gibt an, ob die Zellenformel eine Array‑Formel ist. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Gibt an, ob diese Zelle Teil einer Tabellenformel ist. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Überprüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Gibt an, ob der Wert dieser Zelle numerisch (int, double und datetime) ist |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Gibt an, ob die Zellformel Teil einer gemeinsamen Formel ist. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Gibt an, ob der Zellenstil festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Gibt an, ob diese Zelle Teil einer Tabellenformel ist. |
| [Name](../../aspose.cells/cell/name/) { get; } | Ermittelt den Namen der Zelle. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Stellt den Kategorie‑Typ der Zahlenformatierung dieser Zelle dar. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Ermittelt eine [`Picture`](../../aspose.cells.drawing/picture/) Instanz, die das eingebettete Bild in dieser Zelle darstellt, oder null, wenn für diese Zelle kein eingebettetes Bild vorhanden ist. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Ermittelt oder legt eine R1C1‑Formel der `Cell` fest. |
| [Row](../../aspose.cells/cell/row/) { get; } | Ermittelt die Zeilennummer (nullbasiert) der Zelle. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Ermittelt den Index des geteilten Stils der Zelle im Stil‑Pool. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Ermittelt den Zeichenkettenwert, der in der Zelle enthalten ist. Wenn der Typ dieser Zelle Zeichenkette ist, wird der Zeichenkettenwert selbst zurückgegeben. Für andere Zellentypen wird der formatierte Zeichenkettenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben. Der formatierte Zellenwert entspricht dem, was Sie aus Excel erhalten, wenn Sie eine Zelle als Text kopieren (z. B. das Kopieren einer Zelle in einen Texteditor oder das Exportieren nach CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Ermittelt den Wert der Zelle als Zeichenkette ohne Formatierung. |
| [Type](../../aspose.cells/cell/type/) { get; } | Stellt den Zellenwerttyp dar. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Ermittelt/legt den in dieser Zelle enthaltenen Wert fest. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Ermittelt das übergeordnete Arbeitsblatt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Berechnet die Formel der Zelle. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich innerhalb des Zellentextes darstellt. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Kopiert Daten aus einer Quellzelle. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes Zellenobjekt verweist. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Prüft, ob dieses Objekt auf dieselbe Zelle wie ein anderes verweist. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Ermittelt den Array‑Bereich, wenn die Zellformel eine Array‑Formel ist. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Gibt alle Characters‑Objekte zurück, die einen Zeichenbereich innerhalb des Zellentextes darstellen. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Gibt alle Characters‑Objekte zurück, die einen Zeichenbereich innerhalb des Zellentextes darstellen. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Ermittelt das Ergebnis der bedingten Formatierung. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Ermittelt alle Zellen, deren Formel direkt auf diese Zelle verweist. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Ermittelt alle Zellen, deren berechnetes Ergebnis von dieser Zelle abhängt. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Ermittelt den Anzeigestil dieser Zelle. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Ermittelt den Anzeigestil dieser Zelle. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Ermittelt den Anzeigestil dieser Zelle. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Liefert Formatbedingungen, die für diese Zelle gelten. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Liefert die Formel dieser Zelle. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Dient als Hash-Funktion für einen bestimmten Typ. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Liefert die Höhe des Werts in der Einheit Pixel. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Liefert den HTML-String, der Daten und einige Formate in dieser Zelle enthält. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Liefert alle Zellen, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Liefert alle Zellen, die aktualisiert werden, wenn diese Zelle geändert wird. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Gibt ein [`Range`](../range/)‑Objekt zurück, das einen zusammengeführten Bereich darstellt. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Liefert alle Verweise, die in der Formel dieser Zelle vorkommen. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Liefert alle Vorgänger (Verweise auf Zellen in der aktuellen Arbeitsmappe), die von der Formel dieser Zelle bei deren Berechnung verwendet werden. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Liefert den Rich‑Wert der Zelle. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Liefert den Zeichenkettenwert nach einer spezifischen Formatierungsstrategie. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Liefert den Zellenstil. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Wenn checkBorders true ist, prüfe, ob die Rahmen anderer Zellen den Stil dieser Zelle beeinflussen. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Liefert die Tabelle, die diese Zelle enthält. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Liefert die auf diese Zelle angewendete Validierung. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Liefert den Wert der Validierung, die auf diese Zelle angewendet wurde. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Liefert die Breite des Werts in der Einheit Pixel. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Fügt der Zelle einige Zeichen ein. Wenn die Zelle reich formatiert ist, kann diese Methode die ursprüngliche Formatierung beibehalten. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Schreibt einen booleschen Wert in die Zelle. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Schreibt einen DateTime‑Wert in die Zelle. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Schreibt einen double‑Wert in die Zelle. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Schreibt einen integer‑Wert in die Zelle. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Schreibt einen Objektwert in die Zelle. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Fügt einen Zeichenkettenwert in die Zelle ein. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Fügt einen Zeichenkettenwert in die Zelle ein und konvertiert den Wert bei Bedarf in einen anderen Datentyp. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Fügt einen Wert in die Zelle ein, bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Array-Formel entfernen. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Text der Zelle mit Optionen ersetzen. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Setzt eine Array-Formel (Legacy-Array-Formel, die in MS Excel über STRG+SHIFT+ENTER eingegeben wird) für einen Zellbereich. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Setzt eine Array-Formel für einen Zellbereich. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Setzt eine Array-Formel für einen Zellbereich. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Setzt eine Array-Formel für einen Zellbereich. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Setzt das Rich-Text-Format der Zelle. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Setzt eine dynamische Array-Formel und lässt die Formel, wenn möglich, in benachbarte Zellen überlaufen. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Setzt die Formel und den Wert (berechnetes Ergebnis) der Formel. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Setzt die Formel und den Wert der Formel. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Setzt eine Formel für einen Zellbereich. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Setzt gemeinsam genutzte Formeln für einen Zellbereich. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Setzt den Zellenstil. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Wendet die geänderte Eigenschaft des Stils auf die Zelle an. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Wendet den Zellenstil basierend auf Flags an. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Konvertiert `Cell` in JSON-Strukturdaten. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            // Greift auf die Zellen-Sammlung zu
            Cells cells = worksheet.Cells;

            // Fügt eine Zeichenkette in eine Zelle ein
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Fügt eine Ganzzahl in eine Zelle ein
            cell = cells["B1"];
            cell.PutValue(12);

            // Fügt eine Gleitkommazahl in eine Zelle ein
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Formel in eine Zelle einfügen
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Kombinierte Formel einfügen: "sum(average(b1,c1), b1)" in Zelle b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Stil einer Zelle festlegen
            Style style = cell.GetStyle();
            // Hintergrundfarbe festlegen
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Schriftart einer Zelle festlegen
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



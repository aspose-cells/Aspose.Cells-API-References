---
title: "Klasse SettableGlobalizationSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SettableGlobalizationSettings Klasse. Implementierung von GlobalizationSettings, die es dem Benutzer ermöglicht, vordefinierte Texte festzulegen/zu ändern"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Implementierung von GlobalizationSettings, die es dem Benutzer ermöglicht, vordefinierte Texte festzulegen/zu ändern.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Liest oder setzt die Globalisierungseinstellungen für Diagramm.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in einer Formel. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Liest das Trennzeichen für Listen, Funktionsparameter, ...usw. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Liest oder setzt die Globalisierungseinstellungen für die Pivot-Tabelle.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Liest das Trennzeichen für Zeilen in Array-Daten in einer Formel. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Sortierregeln.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Gibt den Namen des "(All)"-Labels in der PivotTable.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Gibt den Anzeigestringwert für den booleschen Wert einer Zelle zurück. |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Wandelt die Zeichenkette gemäß bestimmter Sortierregeln in ein vergleichbares Objekt um.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Gibt den Namen des "Column Labels"-Labels in der PivotTable.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Gibt den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Kommentar‑Titeltyp zurück. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Gibt den Namen der Feldkopfzeile des Wertebereichs in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Gibt den Standardblattnamen für das automatische Hinzufügen eines Arbeitsblatts zurück. Standard ist "Sheet".(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Gibt den Namen des "(blank)"-Labels in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Gibt den Anzeigestringwert für den Fehlerwert einer Zelle zurück. |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Gibt den Namen des Gesamtsummens der Funktion zurück. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Gibt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext zurück. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Gibt den Namen des "(Multiple Items)"-Labels in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Gibt den Namen des "Grand Total"-Labels in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Gibt den Namen des "Total"-Labels in der PivotTable zurück. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Gibt den Schutznamen in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Gibt den Namen des "Row Labels"-Labels in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Gibt den Standardtext des integrierten Namens gemäß dem gegebenen lokalisierungsabhängigen Text zurück. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Gibt den Standardfunktionsnamen gemäß dem gegebenen lokalisierungsabhängigen Funktionsnamen zurück. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Gibt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf‑/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen zurück. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Gibt den Namen des [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/)-Typs in der PivotTable zurück.(Vererbt von [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Gibt den Typnamen der Tabellenzeilen zurück, die alle Zeilen in der referenzierten Tabelle umfassen. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Gibt den Typnamen der Tabellenzeilen zurück, die die aktuelle Zeile in der referenzierten Tabelle umfassen. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Gibt den Typnamen der Tabellenzeilen zurück, die den Datenbereich der referenzierten Tabelle umfassen. Standard ist "Data", sodass in der Formel "#Data" den Datenbereich der Tabelle darstellt. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Gibt den Typnamen von Tabellenzeilen zurück, die die Tabellenüberschrift enthalten. Standard ist "Headers", sodass in der Formel "#Headers" die Tabellenüberschrift darstellt. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Gibt den Typnamen von Tabellenzeilen zurück, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Gibt den Gesamtnamen einer bestimmten Funktion zurück. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Legt den Anzeigestring‑Wert für den booleschen Wert einer Zelle fest. |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Legt das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in der Formel fest. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Gibt den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Kommentar‑Titeltyp zurück. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Legt den Namen der Gesamtsumme einer bestimmten Funktion fest. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Legt das Trennzeichen für Listen, Funktionsparameter, … usw. fest. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Legt den lokalisierungsabhängigen Text für den integrierten Namen mit dem angegebenen Standardnamen‑Text fest. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Legt den lokalisierungsabhängigen Funktionsnamen fest, der dem angegebenen Standardfunktionsnamen entspricht. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Legt das Trennzeichen für Zeilen in Array‑Daten in der Formel fest. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Legt den Typnamen von Tabellenzeilen fest, die alle Zeilen der referenzierten Tabelle enthalten. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Legt den Typnamen von Tabellenzeilen fest, die die aktuelle Zeile in der referenzierten Tabelle enthalten. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Legt den Typnamen von Tabellenzeilen fest, die den Datenbereich der referenzierten Tabelle enthalten. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Legt den Typnamen von Tabellenzeilen fest, die die Tabellenüberschrift enthalten. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Legt den Typnamen von Tabellenzeilen fest, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Legt den Gesamtnamen einer bestimmten Funktion fest. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Benutzerdefiniertes Listentrennzeichen festlegen
            settings.SetListSeparator(';');

            // Benutzerdefinierte boolesche Wertzeichenketten festlegen
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Benutzerdefinierte Funktionsnamen festlegen
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Benutzerdefinierte Tabellereihen‑Typnamen festlegen
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Benutzerdefinierte Kommentar‑Titelnamen festlegen
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Die Autorzeile wurde entfernt, da CommentTitleType diesen Enum‑Wert nicht hat
            // Wenn Sie autorbezogene Einstellungen festlegen müssen, müssen Sie stattdessen ThreadedCommentAuthor verwenden

            // Wenden Sie die Globalisierungseinstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;

            // Demonstrieren Sie die Verwendung in Formeln
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Speichere die Arbeitsmappe
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



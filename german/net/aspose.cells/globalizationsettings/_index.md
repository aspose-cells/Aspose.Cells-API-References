---
title: "Klasse GlobalizationSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GlobalizationSettings Klasse. Stellt die Globalisierungseinstellungen dar"
type: docs
url: /de/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Stellt die Globalisierungseinstellungen dar.

```csharp
public class GlobalizationSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Liest oder legt die Globalisierungseinstellungen für Diagramme fest. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in einer Formel. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Liest das Trennzeichen für Listen, Funktionsparameter, ...usw. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Liest oder legt die Globalisierungseinstellungen für die Pivot‑Tabelle fest. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Liest das Trennzeichen für Zeilen in Array-Daten in einer Formel. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Vergleicht zwei Zeichenkettenwerte nach bestimmten Sortierregeln. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Gibt den Namen des \"(All)\"-Labels in der PivotTable zurück. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Gibt den Anzeigestringwert für den booleschen Wert einer Zelle zurück. |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Wandelt die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln um. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Gibt den Namen des Labels "Column Labels" in der PivotTable zurück. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Gibt den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Kommentar‑Titeltyp zurück. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Gibt den Namen der Feldüberschrift des Wertebereichs in der PivotTable zurück. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Gibt den Standardblattnamen für das automatische Hinzufügen eines Arbeitsblatts zurück. Standard ist "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Gibt den Namen des Labels "(blank)" in der PivotTable zurück. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Gibt den Anzeigestringwert für den Fehlerwert einer Zelle zurück. |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Gibt den Namen des Gesamtsummens der Funktion zurück. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Gibt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext zurück. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Gibt den Namen des Labels "(Multiple Items)" in der PivotTable zurück. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Gibt den Namen des Labels "Grand Total" in der PivotTable zurück. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Gibt den Namen des Labels "Total" in der PivotTable zurück. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Gibt den Namen des Schutzes in der PivotTable zurück. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Gibt den Namen des Labels "Row Labels" in der PivotTable zurück. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Gibt den Standardtext des integrierten Namens gemäß dem gegebenen lokalisierungsabhängigen Text zurück. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Gibt den Standardfunktionsnamen gemäß dem gegebenen lokalisierungsabhängigen Funktionsnamen zurück. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Gibt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf‑/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen zurück. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Gibt den Namen des Typs [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) in der PivotTable zurück. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Gibt den Typnamen von Tabellenzeilen zurück, die alle Zeilen in der referenzierten Tabelle enthalten. Standard ist "All", sodass in der Formel "#All" alle Zeilen in der referenzierten Tabelle darstellt. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Gibt den Typnamen von Tabellenzeilen zurück, die die aktuelle Zeile in der referenzierten Tabelle enthalten. Standard ist "This Row", sodass in der Formel "#This Row" die aktuelle Zeile in der referenzierten Tabelle darstellt. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Gibt den Typnamen der Tabellenzeilen zurück, die den Datenbereich der referenzierten Tabelle umfassen. Standard ist "Data", sodass in der Formel "#Data" den Datenbereich der Tabelle darstellt. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Gibt den Typnamen von Tabellenzeilen zurück, die die Tabellenüberschrift enthalten. Standard ist "Headers", sodass in der Formel "#Headers" die Tabellenüberschrift darstellt. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Gibt den Typnamen von Tabellenzeilen zurück, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten. Standard ist "Totals", sodass in der Formel "#Totals" die Gesamtsumme‑Zeile der referenzierten Tabelle darstellt. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Gibt den Gesamtnamen der Funktion zurück. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Erstelle und wende Globalisierungseinstellungen an
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Wende Zwischensumme mit benutzerdefinierter Globalisierung an
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Passe den Gesamtnamen basierend auf dem Funktionstyp an
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Klass GlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GlobalizationSettings-klass. Representerar globaliseringsinställningarna"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Representerar globaliseringsinställningarna.

```csharp
public class GlobalizationSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Hämtar eller anger globaliseringsinställningarna för diagram. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Hämtar separatorn för objekten i arrayens raddata i formeln. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Hämtar separatorn för lista, funktionsparametrar, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Hämtar eller anger globaliseringsinställningarna för pivottabellen. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Hämtar separatorn för rader i arraydata i formeln. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Jämför två strängvärden enligt vissa kollationsregler. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Hämtar namnet på "(All)"-etiketten i PivotTable. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Hämtar visningssträngvärdet för cellens booleska värde |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Omvandlar strängen till ett jämförbart objekt enligt vissa kollationsregler. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Hämtar namnet på "Column Labels"-etiketten i PivotTable. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Hämtar namnet på rubriken för värdeområdesfältet i pivottabellen. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Hämtar standardbladnamnet för att automatiskt lägga till ett kalkylblad. Standard är "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Hämtar namnet på etiketten "(blank)" i pivottabellen. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Hämtar visningssträngvärdet för cellens felvärde |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Hämtar namnet på totalen för funktionen. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Hämtar den lokalanpassade texten för inbyggt namn enligt given standardtext. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Hämtar det lokalanpassade funktionsnamnet enligt given standardfunktionsnamn. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Hämtar namnet på etiketten "(Multiple Items)" i pivottabellen. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Hämtar namnet på etiketten "Grand Total" i pivottabellen. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Hämtar namnet på etiketten "Total" i pivottabellen. Du måste åsidosätta den här metoden när pivottabellen innehåller två eller fler PivotFields i dataområdet. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Hämtar skyddsnamnet i pivottabellen. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Hämtar namnet på etiketten "Row Labels" i pivottabellen. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Hämtar standardtexten för inbyggt namn enligt given lokalanpassad text. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Hämtar standardfunktionsnamnet enligt givet lokalanpassat funktionsnamn. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Hämtar standardengelskt teckensnittsstilsnamn (Regular, Bold, Italic) för Header/Footer enligt given lokalanpassat teckensnittsstilsnamn. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Hämtar namnet på typen [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) i pivottabellen. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. Standard är "All", så i formeln "#All" representerar alla rader i den refererade tabellen. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. Standard är "This Row", så i formeln "#This Row" representerar den aktuella raden i den refererade tabellen. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Hämtar typnamnet för tabellrader som består av datatområdet i den refererade tabellen. Standard är "Data", så i formeln "#Data" representerar datatområdet i tabellen. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. Standard är "Totals", så i formeln "#Totals" representerar totalraden i den refererade tabellen. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Hämtar totalnamnet för funktionen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
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

            // Skapa och tillämpa globaliseringsinställningar
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Tillämpa delsumma med anpassad globalisering
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Anpassa totalnamnet baserat på funktionstyp
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



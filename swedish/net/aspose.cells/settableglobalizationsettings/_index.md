---
title: "Klass SettableGlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SettableGlobalizationSettings klass. Implementering av GlobalizationSettings som stödjer användaren att ange/ändra fördefinierade texter"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Implementering av GlobalizationSettings som låter användaren ange/ändra fördefinierade texter.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Hämtar eller anger globaliseringsinställningarna för Diagram.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Hämtar separatorn för objekten i arrayens raddata i formeln. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Hämtar separatorn för lista, funktionsparametrar, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Hämtar eller anger globaliseringsinställningarna för pivottabellen.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Hämtar separatorn för rader i arraydata i formeln. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Jämför två strängvärden enligt vissa sorteringsregler.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Föråldrad.**) Hämtar namnet på etiketten "(All)" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Hämtar visningssträngvärdet för cellens booleska värde |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Föråldrad.**) Hämtar namnet på etiketten "Column Labels" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Föråldrad.**) Hämtar namnet på fältrubriken för värdeområdet i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Hämtar standardbladnamnet för att automatiskt lägga till kalkylblad. Standard är "Sheet".(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Föråldrad.**) Hämtar namnet på etiketten "(blank)" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Hämtar visningssträngvärdet för cellens felvärde |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Hämtar namnet på totalen för funktionen. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Hämtar den lokalanpassade texten för inbyggt namn enligt given standardtext. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Hämtar det lokalanpassade funktionsnamnet enligt given standardfunktionsnamn. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Föråldrad.**) Hämtar namnet på etiketten "(Multiple Items)" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Föråldrad.**) Hämtar namnet på etiketten "Grand Total" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Föråldrad.**) Hämtar namnet på etiketten "Total" i PivotTable. Du måste åsidosätta denna metod när PivotTable innehåller två eller fler PivotFields i dataområdet.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Föråldrad.**) Hämtar skyddsnamnet i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Föråldrad.**) Hämtar namnet på etiketten "Row Labels" i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Hämtar standardtexten för inbyggt namn enligt given lokalanpassad text. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Hämtar standardfunktionsnamnet enligt givet lokalanpassat funktionsnamn. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Hämtar standardengelskt teckensnittsstilsnamn (Regular, Bold, Italic) för Header/Footer enligt given lokalanpassat teckensnittsstilsnamn. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Föråldrad.**) Hämtar namnet på typen [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) i PivotTable.(Ärvd från [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Hämtar typnamnet för tabellrader som består av datatområdet i den refererade tabellen. Standard är "Data", så i formeln "#Data" representerar datatområdet i tabellen. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Hämtar totalnamnet för en specifik funktion. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Ställer in visningssträngvärdet för cellens booleska värde |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Ställer in separatorn för objekten i arrayens raddata i formeln. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Ställer in det samlade totalnamnet för en specifik funktion. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Ställer in separatorn för list, parameters of function, ...etc. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Ställer in den lokalberoende texten för det inbyggda namnet med given standard name text. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Ställer in det lokalberoende funktionsnamnet som motsvarar det givna standardfunktionsnamnet. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Ställer in separatorn för rader i array data i formeln. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Ställer in typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Ställer in typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Ställer in typnamnet för tabellrader som består av datatområdet i den refererade tabellen. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Ställer in typnamnet för tabellrader som består av tabellhuvudet. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Ställer in typnamnet för tabellrader som består av totalraden i den refererade tabellen. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Ställer in totalnamnet för en specifik funktion. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Ange anpassad listseparator
            settings.SetListSeparator(';');

            // Ange anpassade booleska värdesträngar
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Ange anpassade funktionsnamn
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Ange anpassade typnamn för tabellrader
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Ange anpassade kommentarsrubriknamn
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Tog bort författarlinjen eftersom CommentTitleType inte har det enum‑värdet
            // Om du behöver ställa in författarrelaterade inställningar måste du använda ThreadedCommentAuthor istället

            // Applicera globaliseringsinställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            // Visa användning i formler
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Klass WorkbookDesigner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WorkbookDesigner-klass. Inkapslar objektet som representerar ett designer-kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Inkapslar objektet som representerar ett designkalkylblad.

```csharp
public class WorkbookDesigner
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Initierar en ny instans av klassen `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Initierar en ny instans av klassen `WorkbookDesigner`. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Anger om formler ska beräknas. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Hämtar och anger återuppringningsgränssnitt för bearbetning av smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Anger om det första kalkylbladet innehåller anpassade variabler. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Anger om sidhuvud/sidfot innehåller smarta markörer och bör bearbetas tillsammans. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Anger om bearbetning av den smarta markören sker rad för rad. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Anger om formler ska upprepas med en delrad. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Indikerar om datakällan sorteras. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Om TRUE, infogas Null om värdet är ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Anger om referenser i andra kalkylblad kommer att uppdateras. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Hämtar och anger namnet på kalkylbladet som innehåller variabler för smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Hämtar och anger [`Workbook`](./workbook/)‑objektet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Rensar alla datakällor. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Returnerar en samling av smart markers i ett kalkylblad. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Bearbetar smart markers och fyller i värdena för datakällan. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Bearbetar smart markers och fyller i värdena för datakällan. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) Bearbetar smart markers och fyller i värdena för datakällan. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Anger datakälla för ett DataSet‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Anger datakälla för ett DataTable‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Anger datakälla för ett DataView‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Anger datakälla för ett OleDbConnection‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Anger datakälla för ett SqlConnection‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Anger datakälla för ett DataView‑objekt och binder det till ett datakällnamn. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Anger datakälla för ett [`ICellsDataTable`](../icellsdatatable/)‑objekt. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Anger databindning till en variabel. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Anger datakälla för ett IDataReader‑objekt. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Ange JSON‑strängvärde som datakälla för smart markers. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // Skapa WorkbookDesigner‑objekt
            WorkbookDesigner wd = new WorkbookDesigner();

            // Öppna mallfilen (som innehåller smart markers)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Initiera dina data från datakällan
            DataSet ds = new DataSet();
            // Lägg till data i datasetet (detta är bara ett exempel, ersätt med faktisk datakälla)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Ange datasetet som datakälla
            wd.SetDataSource(ds);

            // Bearbeta smart markers för att fylla i data i kalkylbladen
            wd.Process(true);

            // Spara Excel-filen
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Visar andra egenskaper
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Rensa datakälla
            wd.ClearDataSource();

            // Ange datakälla med olika metoder
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Bearbeta smart markers igen
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Spara Excel-filen igen
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



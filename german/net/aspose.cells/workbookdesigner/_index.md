---
title: "Klasse WorkbookDesigner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WorkbookDesigner-Klasse. Kapselt das Objekt, das eine Designer-Tabellenkalkulation darstellt"
type: docs
url: /de/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Kapselt das Objekt, das ein Designer‑Spreadsheet darstellt.

```csharp
public class WorkbookDesigner
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Initialisiert eine neue Instanz der `WorkbookDesigner`-Klasse. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Initialisiert eine neue Instanz der `WorkbookDesigner`-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Gibt an, ob Formeln berechnet werden sollen. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Liest und setzt die Callback-Schnittstelle für die Verarbeitung von Smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Gibt an, ob Kopf-/Fußzeile Smartmarker enthält und gemeinsam verarbeitet werden soll. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Gibt an, ob die Verarbeitung des Smartmarkers zeilenweise erfolgt. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Gibt an, ob die Datenquelle sortiert wird. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Liest und setzt den Namen des Arbeitsblatts, das Variablen‑Smart‑Marker enthält. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Liest und setzt das [`Workbook`](./workbook/)‑Objekt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Löscht alle Datenquellen. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Gibt eine Sammlung von Smart‑Markern in einer Tabellenkalkulation zurück. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Veraltet.**) Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Setzt die Datenquelle eines DataSet‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Setzt die Datenquelle eines DataTable‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Setzt die Datenquelle eines DataView‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Setzt die Datenquelle eines OleDbConnection‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Setzt die Datenquelle eines SqlConnection‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Setzt die Datenquelle eines DataView‑Objekts und bindet sie an einen Datenquellennamen. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Setzt die Datenquelle eines [`ICellsDataTable`](../icellsdatatable/)‑Objekts. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Setzt die Datenbindung zu einer Variablen. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Setzt die Datenquelle eines IDataReader‑Objekts. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Setzt den JSON‑Stringwert als Datenquelle für Smart‑Marker. |

### Beispiele

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
            // Erstelle WorkbookDesigner‑Objekt
            WorkbookDesigner wd = new WorkbookDesigner();

            // Öffne die Vorlagendatei (die Smart‑Marker enthält)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Initialisieren Sie Ihre Daten aus der Datenquelle
            DataSet ds = new DataSet();
            // Füge Daten zum Dataset hinzu (dies ist nur ein Beispiel, ersetze es durch die tatsächliche Datenquelle)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Setze das Dataset als Datenquelle
            wd.SetDataSource(ds);

            // Verarbeiten Sie die Smartmarker, um die Daten in die Arbeitsblätter einzufügen
            wd.Process(true);

            // Speichere die Excel-Datei
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Demonstration weiterer Eigenschaften
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Lösche Datenquelle
            wd.ClearDataSource();

            // Setze Datenquelle mit verschiedenen Methoden
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Verarbeite die Smart‑Marker erneut
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Speichere die Excel‑Datei erneut
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "OdsLoadOptions.IsClassicPivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsLoadOptions-Eigenschaft. Gibt an, ob die Pivot-Tabelle klassisch ist"
type: docs
url: /de/net/aspose.cells/odsloadoptions/isclassicpivottable/
---
## OdsLoadOptions.IsClassicPivotTable property

Gibt an, ob die Pivot‑Tabelle klassisch ist.

```csharp
public bool IsClassicPivotTable { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-ODS-Datei mit Pivot-Tabelle
            CreateSampleOdsWithPivotTable();

            // Lade mit IsClassicPivotTable auf true gesetzt
            OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
            loadOptionsTrue.IsClassicPivotTable = true;
            
            Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
            Console.WriteLine("Loaded with IsClassicPivotTable = true");
            Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);

            // Lade mit IsClassicPivotTable auf false gesetzt
            OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
            loadOptionsFalse.IsClassicPivotTable = false;
            
            Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
            Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
            Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
        }

        private static void CreateSampleOdsWithPivotTable()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten befüllen
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Electronics";
            cells["A3"].Value = "Clothing";
            cells["A4"].Value = "Books";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 800;
            cells["B4"].Value = 200;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Füge Zeilenfeld (Category) hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Füge Datenfeld (Sales) hinzu und setze den Anzeigenamen
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";

            // Als ODS speichern
            workbook.Save("SamplePivot.ods", SaveFormat.Ods);
        }
    }
}
```

### Siehe auch

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



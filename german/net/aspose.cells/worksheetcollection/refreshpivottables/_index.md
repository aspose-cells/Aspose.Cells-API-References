---
title: "WorksheetCollection.RefreshPivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Aktualisiert alle PivotTables in der Excel-Datei"
type: docs
url: /de/net/aspose.cells/worksheetcollection/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Aktualisiert alle PivotTables in der Excel-Datei.

```csharp
public void RefreshPivotTables()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // PivotTable hinzufügen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Quellendaten ändern
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Aktualisiere alle PivotTables in der Arbeitsmappe.
            workbook.Worksheets.RefreshPivotTables();

            // Speichere die Arbeitsmappe
            workbook.Save("RefreshPivotTablesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Aktualisiert alle PivotTables in der Excel-Datei.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Option | PivotTableRefreshOption | Die Option zum Aktualisieren der Datenquelle der PivotTables. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 2300;

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotTableRefreshOption option = new PivotTableRefreshOption();

            workbook.Worksheets.RefreshPivotTables(option);

            Console.WriteLine(cells["F8"].StringValue);

            cells["B2"].Value = 2000;

            workbook.Worksheets.RefreshPivotTables(option);
            Console.WriteLine(cells["F8"].StringValue);
                       


            workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



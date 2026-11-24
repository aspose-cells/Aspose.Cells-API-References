---
title: "PivotTableCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableCollection-Eigenschaft. Gibt den PivotTable-Bericht nach Index zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Ermittelt den PivotTable-Bericht nach Index.

```csharp
public PivotTable this[int index] { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Ein Arbeitsbuch aus einer Quelldatei erstellen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf die PivotTable-Sammlung
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Zugriff auf die erste PivotTable über die Item-Eigenschaft (Indexer)
            PivotTable pivotTable = pivotTables[0];
            
            // PivotTable-Daten berechnen
            pivotTable.CalculateData();
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Ermittelt den PivotTable-Bericht anhand des Namens der PivotTable.

```csharp
public PivotTable this[string name] { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTable konfigurieren über die Item-Eigenschaft
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktualisieren und Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Zugriff auf die PivotTable über die Item-Eigenschaft
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Daten ändern und aktualisieren
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Ermittelt die [`PivotTable`](../../pivottable/), die sich in der Zelle befindet.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Zugriff auf die PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Demonstration des Zugriffs auf eine PivotTable über die Item-Eigenschaft (Indexer)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Demonstration des Zugriffs per Name über die Item-Eigenschaft
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // PivotTable konfigurieren
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Aktualisieren und Daten berechnen
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Speichere die Arbeitsmappe
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



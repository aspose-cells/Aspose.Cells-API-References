---
title: "Klasse DataModelTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataModels.DataModelTable Klasse. Stellt Eigenschaften einer einzelnen Tabelle im Tabellenkalkulationsdatenmodell dar"
type: docs
url: /de/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Stellt Eigenschaften einer einzelnen Tabelle im Datenmodell der Tabellenkalkulation dar.

```csharp
public class DataModelTable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Ermittelt den Verbindungsnamen der Datenmodell-Tabelle. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Ermittelt die ID der Datenmodell-Tabelle. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Ermittelt den Namen der Datenmodell-Tabelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Erstelle ein ListObject (Tabelle)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Greife auf die DataModelTable zu
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Zeige DataModelTable-Eigenschaften an
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Erstellen Sie eine Pivot-Tabelle mit dem DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)



---
title: "DataModelTable.ConnectionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelTable-Eigenschaft. Gibt den Verbindungsnamen der Datenmodell-Tabelle zurück"
type: docs
url: /de/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Ermittelt den Verbindungsnamen der Datenmodell-Tabelle.

```csharp
public string ConnectionName { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Erstelle ein ListObject (Tabelle)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Greife auf die DataModelTable zu
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Anzeige des aktuellen ConnectionName-Werts
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Erstelle eine Pivot-Tabelle unter Verwendung der Verbindung der DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Hinweis: ConnectionName ist schreibgeschützt, daher können wir sie nicht setzen
            // Dies zeigt, wie man den vorhandenen Verbindungsnamen verwendet
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)



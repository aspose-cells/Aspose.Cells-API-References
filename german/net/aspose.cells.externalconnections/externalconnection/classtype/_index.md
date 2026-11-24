---
title: "ExternalConnection.ClassType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Gibt den Typ dieses ExternalConnection-Objekts zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Gibt den Typ dieses [`ExternalConnection`](../)-Objekts zurück.

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Erstellen Sie eine Pivot-Tabelle mit Data Model-Verbindung
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Holen Sie die externe Verbindung und demonstrieren Sie die ClassType-Eigenschaft
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // Speichere die Arbeitsmappe
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)



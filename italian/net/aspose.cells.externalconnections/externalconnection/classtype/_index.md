---
title: "ExternalConnection.ClassType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene il tipo di questo oggetto ExternalConnection"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Ottiene il tipo di questo oggetto [`ExternalConnection`](../).

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Crea una tabella pivot con connessione al modello dati
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ottieni la connessione esterna e dimostra la proprietà ClassType
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // Salva la cartella di lavoro
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)



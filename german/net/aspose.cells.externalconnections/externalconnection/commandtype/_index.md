---
title: "ExternalConnection.CommandType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Gibt den OLE DB-Befehlstyp an. 1. Query gibt einen Würfelnamen an 2. Query gibt eine SQL-Anweisung an 3. Query gibt einen Tabellennamen an 4. Query gibt an, dass Standardinformationen bereitgestellt wurden und es dem Provider überlassen ist, wie er sie interpretiert. 5. Query erfolgt gegen einen webbasierten List Data Provider."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Gibt den OLE DB-Befehlstyp an. 1. Abfrage gibt einen Würfelnamen an 2. Abfrage gibt eine SQL-Anweisung an 3. Abfrage gibt einen Tabellennamen an 4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese interpretiert werden. 5. Abfrage erfolgt gegen einen webbasierten List Data Provider.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Hole die externe Verbindung
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // CommandType-Eigenschaft demonstrieren
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // CommandType ändern und anzeigen
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)



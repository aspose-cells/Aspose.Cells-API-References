---
title: "DataModelTable.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelTable-Eigenschaft. Gibt die ID der Datenmodell-Tabelle zurück"
type: docs
url: /de/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Ermittelt die ID der Datenmodell-Tabelle.

```csharp
public string Id { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Erstelle ein ListObject (Tabelle)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Abrufen der DataModelTable (dies ist im Arbeitsbuch schreibgeschützt)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Anzeige des aktuellen ID-Werts
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Hinweis: Die Id-Eigenschaft ist schreibgeschützt, daher können wir sie nicht setzen
            // Dies zeigt, wie man die vorhandene Id zugreift und verwendet

            // Beispielhafte Verwendung: Tabellen-IDs vergleichen, wenn mit mehreren Tabellen gearbeitet wird
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)



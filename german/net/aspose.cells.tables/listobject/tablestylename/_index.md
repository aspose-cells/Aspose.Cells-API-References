---
title: "ListObject.TableStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt den Tabellestilnamen zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Ermittelt und setzt den Tabellenvorlagennamen.

```csharp
public string TableStyleName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Ein Listenobjekt/Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Tabellestil festlegen und anzeigen
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



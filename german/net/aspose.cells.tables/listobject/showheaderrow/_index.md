---
title: "ListObject.ShowHeaderRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt an und legt fest, ob diese Tabelle die Kopfzeile anzeigt"
type: docs
url: /de/net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Ermittelt und setzt, ob diese Tabelle die Kopfzeile anzeigt.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowHeaderRowDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und ein Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Ein Listenobjekt/Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            table.ShowHeaderRow = true; // Header row is visible by default

            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Kopfzeile ausblenden
            table.ShowHeaderRow = false;
            Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



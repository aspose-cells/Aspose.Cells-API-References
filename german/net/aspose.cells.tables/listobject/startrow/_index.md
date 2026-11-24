---
title: "ListObject.StartRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt die Startzeile des Bereichs zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Ermittelt die Startzeile des Bereichs.

```csharp
public int StartRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten ab Zeile 2 erstellen
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Ein ListObject ab Zeile 2 erstellen
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Zeige die StartRow-Eigenschaft an
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // Um die Startzeile zu "ändern", müssen wir das ListObject neu erstellen
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



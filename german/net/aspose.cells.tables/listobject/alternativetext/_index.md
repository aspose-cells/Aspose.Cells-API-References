---
title: "ListObject.AlternativeText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject‑Eigenschaft. Ruft den Alternativtext ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Liest und setzt den alternativen Text.

```csharp
public string AlternativeText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
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
            
            // Alternativen Text und Beschreibung festlegen
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Neu laden und überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



---
title: "ListObject.AlternativeDescription"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject property. Ruft die alternative Beschreibung ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Liest und setzt die alternative Beschreibung.

```csharp
public string AlternativeDescription { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
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

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Alternativen Text und Beschreibung festlegen
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Eigenschaften neu laden und überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



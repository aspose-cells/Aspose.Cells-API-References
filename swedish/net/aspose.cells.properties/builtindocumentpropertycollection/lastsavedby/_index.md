---
title: "BuiltInDocumentPropertyCollection.LastSavedBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger namnet på den sista författaren"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedby/
---
## BuiltInDocumentPropertyCollection.LastSavedBy property

Hämtar eller anger namnet på den senaste författaren.

```csharp
public string LastSavedBy { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in inbyggda dokumentegenskaper inklusive LastSavedBy
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";
            workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
            
            // Spara arbetsboken
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
            
            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
            
            // Skriv ut LastSavedBy-egenskapen
            Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



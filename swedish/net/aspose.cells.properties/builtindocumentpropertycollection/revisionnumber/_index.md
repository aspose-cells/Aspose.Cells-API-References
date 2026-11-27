---
title: "BuiltInDocumentPropertyCollection.RevisionNumber"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection property. Hämtar eller anger dokumentets revisionsnummer"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

Hämtar eller anger dokumentets revisionsnummer.

```csharp
public string RevisionNumber { get; set; }
```

### Anmärkningar

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange RevisionNumber‑egenskapen
            workbook.BuiltInDocumentProperties.RevisionNumber = "1";
            
            // Visa RevisionNumber
            Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



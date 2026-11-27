---
title: "BuiltInDocumentPropertyCollection.Subject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Hämtar eller anger ämnet för dokumentet"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

Hämtar eller anger ämnet för dokumentet.

```csharp
public string Subject { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in inbyggda dokumentegenskaper
            workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
            workbook.BuiltInDocumentProperties.Title = "LiteraTest";

            // Spara arbetsboken
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            using (Workbook loadedWorkbook = new Workbook(outputPath))
            {
                string subject = loadedWorkbook.BuiltInDocumentProperties.Subject;
                string title = loadedWorkbook.BuiltInDocumentProperties.Title;

                Console.WriteLine("Subject: " + subject);
                Console.WriteLine("Title: " + title);
            }
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



---
title: "BuiltInDocumentPropertyCollection.Subject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Ottiene o imposta l'oggetto del documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

Ottiene o imposta l'oggetto del documento.

```csharp
public string Subject { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le proprietà integrate del documento
            workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
            workbook.BuiltInDocumentProperties.Title = "LiteraTest";

            // Salva la cartella di lavoro
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare le proprietà
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

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



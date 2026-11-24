---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Liest oder setzt den Namen des Autors des Dokuments"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Ermittelt oder setzt den Namen des Autors des Dokuments.

```csharp
public string Author { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Autor-Eigenschaft festlegen
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Zeige die author-Eigenschaft an
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



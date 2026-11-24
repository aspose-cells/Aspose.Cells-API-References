---
title: "BuiltInDocumentPropertyCollection.NameOfApplication"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection property. Gibt den Namen der Anwendung zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Liest oder setzt den Namen der Anwendung.

```csharp
public string NameOfApplication { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die NameOfApplication-Eigenschaft
            workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
            
            // Zeige die NameOfApplication-Eigenschaft an
            Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.ods");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Ruft die Sprache des Dokuments ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Liest oder setzt die Sprache des Dokuments.

```csharp
public string Language { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierte Sammlung von Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Die language-Eigenschaft festlegen
            builtInProperties.Language = "en-US";

            // Weitere grundlegende Eigenschaften zur Demonstration festlegen
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Speichere die Arbeitsmappe
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



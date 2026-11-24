---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Ruft den Informationsnamen der Dokumentvorlage ab oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Liest oder setzt den informativen Namen der Dokumentvorlage.

```csharp
public string Template { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die integrierten Dokumenteigenschaften
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Setzen Sie die Template-Eigenschaft
            builtInProperties.Template = "Standard Template";

            // Weitere grundlegende Eigenschaften zur Demonstration festlegen
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Speichere die Arbeitsmappe
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



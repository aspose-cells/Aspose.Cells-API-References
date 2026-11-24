---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BuiltInDocumentPropertyCollection-Eigenschaft. Gibt den Anzeigemodus der Dokumentvorschau an"
type: docs
url: /de/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Gibt den Anzeigemodus der Dokumentvorschau an.

```csharp
public bool ScaleCrop { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf integrierte Dokumenteigenschaften
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Setze die ScaleCrop-Eigenschaft
            properties.ScaleCrop = true;
            
            // Zeige den Wert der ScaleCrop-Eigenschaft an
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



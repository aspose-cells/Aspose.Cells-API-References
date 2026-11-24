---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookMetadata-Eigenschaft. Gibt eine DocumentProperty-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt"
type: docs
url: /de/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Gibt eine [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/)‑Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Quell- und Zielpfade
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Erstelle Metadatenoptionen für Dokumenteigenschaften
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Initialisiere Arbeitsmappen-Metadaten
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Füge eine benutzerdefinierte Dokumenteigenschaft hinzu
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Speichere die Arbeitsmappe mit Metadaten
            meta.Save(destPath);
            
            // Überprüfe die benutzerdefinierte Eigenschaft
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Siehe auch

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)



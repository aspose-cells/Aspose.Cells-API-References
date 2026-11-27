---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookMetadata‑egenskap. Returnerar en DocumentProperty‑samling som representerar alla anpassade dokumentegenskaper i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Returnerar en [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Exempel

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
            // Käll- och destinationssökvägar
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Skapa metadataalternativ för dokumentegenskaper
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Initiera arbetsbokens metadata
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Lägg till anpassad dokumentegenskap
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Spara arbetsboken med metadata
            meta.Save(destPath);
            
            // Verifiera den anpassade egenskapen
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### Se även

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)



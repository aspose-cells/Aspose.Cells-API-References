---
title: "MetadataOptions.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MetadataOptions-Eigenschaft. Stellt das Verschlüsselungspasswort für die Arbeitsmappe dar"
type: docs
url: /de/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar.

```csharp
public string Password { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Erstellen Sie Metadatenoptionen mit Passwortschutz
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // Erstellen Sie eine neue Arbeitsmappe und speichern Sie sie zuerst
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // Laden Sie Metadaten aus der gespeicherten Datei
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // Füge eine benutzerdefinierte Dokumenteigenschaft hinzu
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Speichern mit Metadaten
            metadata.Save(filePath);
        }
    }
}
```

### Siehe auch

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)



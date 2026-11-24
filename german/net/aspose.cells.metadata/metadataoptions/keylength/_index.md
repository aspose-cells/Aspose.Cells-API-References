---
title: "MetadataOptions.KeyLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MetadataOptions-Eigenschaft. Die Schlüssellänge"
type: docs
url: /de/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

Die Schlüssellänge.

```csharp
public int KeyLength { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // Erstellen Sie Metadatenoptionen mit dem Typ Dokumenteigenschaften
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Legen Sie Verschlüsselungseigenschaften fest, einschließlich KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // Erstellen Sie Metadaten für eine neue Arbeitsmappe
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // Benutzerdefinierte Eigenschaft hinzufügen
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // Speichern mit Verschlüsselung
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### Siehe auch

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)



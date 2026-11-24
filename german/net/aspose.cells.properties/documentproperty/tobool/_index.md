---
title: "DocumentProperty.ToBool"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Methode. Gibt den Eigenschaftswert als bool zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Gibt den Eigenschaftswert als bool zurück.

```csharp
public bool ToBool()
```

### Hinweise

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Boolean ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Eine boolesche benutzerdefinierte Dokumenteigenschaft hinzufügen
            customProperties.Add("IsApproved", true);
            
            // Die Eigenschaft abrufen und mit ToBool() in bool konvertieren
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



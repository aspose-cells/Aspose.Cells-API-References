---
title: "DocumentProperty.ToInt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Methode. Gibt den Eigenschaftswert als Ganzzahl zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Gibt den Eigenschaftswert als integer zurück.

```csharp
public int ToInt()
```

### Hinweise

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Number ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Hole die Sammlung benutzerdefinierter Dokumenteigenschaften
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Füge eine numerische benutzerdefinierte Eigenschaft hinzu
            customProperties.Add("Revision", 5);

            // Hole die Eigenschaft und konvertiere sie mit ToInt() zu int
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Gib das Ergebnis aus
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



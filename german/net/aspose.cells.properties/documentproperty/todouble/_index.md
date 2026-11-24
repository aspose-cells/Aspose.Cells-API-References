---
title: "DocumentProperty.ToDouble"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentProperty-Methode. Gibt den Eigenschaftswert als double zurück"
type: docs
url: /de/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Gibt den Eigenschaftswert als double zurück.

```csharp
public double ToDouble()
```

### Hinweise

Wirft eine Ausnahme, wenn der Eigenschaftstyp nicht PropertyType.Float ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Abrufen der Sammlung benutzerdefinierter Dokumenteigenschaften
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Füge eine numerische Eigenschaft hinzu
            customProperties.Add("Rating", 4.75);

            // Rufe die Eigenschaft ab und konvertiere sie zu double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Gib das Ergebnis aus
            Console.WriteLine($"Rating: {ratingValue}");

            // Speichere die Arbeitsmappe
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



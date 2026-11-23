---
title: "PasteOptions.PasteType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. Le type de collage spécial"
type: docs
url: /fr/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Le type de collage spécial.

```csharp
public PasteType PasteType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur source
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Créer des plages avec des noms de type entièrement qualifiés
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Copier avec PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Afficher les résultats
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Voir aussi

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



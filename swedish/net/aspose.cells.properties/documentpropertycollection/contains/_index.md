---
title: "DocumentPropertyCollection.Contains"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentPropertyCollection‑metod. Returnerar true om en egenskap med det angivna namnet finns i samlingen"
type: docs
url: /sv/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Returnerar true om en egenskap med det angivna namnet finns i samlingen.

```csharp
public bool Contains(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Det skiftlägesokänsliga namnet på egenskapen. |

### Returvärde

True om egenskapen finns i samlingen; false annars.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kontrollera om egenskapen "RevisionNumber" finns i inbyggda dokumentegenskaper
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Lägg till en anpassad egenskap och kontrollera dess existens
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Se även

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



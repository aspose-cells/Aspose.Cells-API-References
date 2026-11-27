---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BuiltInDocumentPropertyCollection egenskap. Returnerar ett DocumentProperty-objekt baserat på egenskapens namn"
type: docs
url: /sv/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Returnerar ett [`DocumentProperty`](../../documentproperty/)-objekt baserat på egenskapens namn.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Det skiftlägesokänsliga namnet på egenskapen som ska hämtas. |

### Anmärkningar

Strängnamnen på egenskaperna motsvarar namnen på de typade egenskaper som finns tillgängliga från [`BuiltInDocumentPropertyCollection`](../).

Om du begär en egenskap som inte finns i dokumentet, men egenskapens namn känns igen som ett giltigt inbyggt namn, skapas en ny [`DocumentProperty`](../../documentproperty/), läggs till i samlingen och returneras. Den nyss skapade egenskapen tilldelas ett standardvärde (tom sträng, noll, falskt eller DateTime.MinValue beroende på typen av den inbyggda egenskapen).

Om du begär en egenskap som inte finns i dokumentet och namnet inte känns igen som ett inbyggt namn, returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in en inbyggd dokumentegenskap med rätt metod
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Åtkomst och skriv ut egenskapsvärdet
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken och verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



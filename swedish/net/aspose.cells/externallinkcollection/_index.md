---
title: "Klass ExternalLinkCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalLinkCollection-klass. Representerar en samling externa länkar i en arbetsbok"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Representerar samlingen av externa länkar i en arbetsbok.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Hämtar antalet element som faktiskt finns i samlingen. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Hämtar [`ExternalLink`](../externallink/) elementet på det angivna indexet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Lägger till en extern länk. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Lägg till en extern länk. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Tar bort alla externa länkar. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Tar bort alla externa länkar. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Hämta en enumerator som itererar genom denna samling. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Tar bort den angivna externa länken från arbetsboken. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Tar bort den angivna externa länken från arbetsboken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Öppna en fil med externa länkar
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Hämta samlingen av externa länkar
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Visa antalet externa länkar
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Iterera genom de externa länkarna och visa deras datakällor
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Lägg till en ny extern länk
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Ändra datakällan för den första externa länken
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Spara arbetsboken
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Rensa alla externa länkar
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Spara arbetsboken efter att ha rensat externa länkar
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



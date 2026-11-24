---
title: "Klasse ExternalLinkCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalLinkCollection Klasse. Stellt die Sammlung externer Links in einer Arbeitsmappe dar."
type: docs
url: /de/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Stellt die Sammlung externer Links in einem Arbeitsblatt dar.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Ermittelt die tatsächlich in der Sammlung enthaltene Anzahl von Elementen. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Ermittelt das [`ExternalLink`](../externallink/) Element am angegebenen Index. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Fügt einen externen Link hinzu. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Fügen Sie einen externen Link hinzu. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Entfernt alle externen Links. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Entfernt alle externen Links. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Holen Sie einen Enumerator, der durch diese Sammlung iteriert. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Entfernt den angegebenen externen Link aus der Arbeitsmappe. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Entfernt den angegebenen externen Link aus der Arbeitsmappe. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Öffnen Sie eine Datei mit externen Links
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Holen Sie die Sammlung externer Links
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Zeigen Sie die Anzahl externer Links an
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Iterieren Sie durch die externen Links und zeigen Sie deren Datenquellen an
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Fügen Sie einen neuen externen Link hinzu
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Ändern Sie die Datenquelle des ersten externen Links
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Alle externen Links löschen
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Speichern Sie die Arbeitsmappe, nachdem die externen Links gelöscht wurden
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



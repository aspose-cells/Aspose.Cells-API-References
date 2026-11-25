---
title: "Classe ExternalLinkCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalLinkCollection. Rappresenta la raccolta di collegamenti esterni in una cartella di lavoro"
type: docs
url: /it/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Rappresenta la raccolta di collegamenti esterni in una cartella di lavoro.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Ottiene il numero di elementi effettivamente contenuti nella raccolta. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Ottiene l'elemento [`ExternalLink`](../externallink/) all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Aggiunge un collegamento esterno. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Aggiungi un collegamento esterno. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Rimuove tutti i collegamenti esterni. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Rimuove tutti i collegamenti esterni. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Ottieni un enumeratore che itera attraverso questa raccolta. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Rimuove il collegamento esterno specificato dalla cartella di lavoro. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Rimuove il collegamento esterno specificato dalla cartella di lavoro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Apri un file con collegamenti esterni
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Ottieni la raccolta di collegamenti esterni
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Visualizza il conteggio dei collegamenti esterni
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Itera attraverso i collegamenti esterni e visualizza le loro fonti dati
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Aggiungi un nuovo collegamento esterno
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Modifica la fonte dati del primo collegamento esterno
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Salva la cartella di lavoro
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Cancella tutti i collegamenti esterni
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Salva la cartella di lavoro dopo aver rimosso i collegamenti esterni
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



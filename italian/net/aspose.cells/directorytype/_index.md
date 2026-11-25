---
title: "Enum DirectoryType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DirectoryType enum. Rappresenta il tipo di directory del nome file"
type: docs
url: /it/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Rappresenta il tipo di directory del nome file.

```csharp
public enum DirectoryType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Volume | `0` | Rappresenta una lettera di unità MS-DOS. È seguita dalla lettera di unità. Oppure nomi di file UNC, come \\server\share\myfile.xls |
| SameVolume | `1` | Indica che la cartella di lavoro di origine si trova sulla stessa unità della cartella di lavoro dipendente (la lettera dell'unità è omessa) |
| DownDirectory | `2` | Indica che la cartella di lavoro di origine è in una sottocartella della directory corrente. |
| UpDirectory | `3` | Indica che la cartella di lavoro di origine è nella directory padre della directory corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Aggiungi un collegamento esterno alla cartella di lavoro
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Aggiungi collegamento esterno con DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Recupera il collegamento esterno aggiunto
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Restituisci i dettagli del collegamento esterno
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Salva la cartella di lavoro
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



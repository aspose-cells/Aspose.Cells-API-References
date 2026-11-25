---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConditionalFormattingIcon. Ottiene i dati dell'immagine con l'impostazione della cella"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Ottiene i dati dell'immagine con l'impostazione della cella.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cella | Cella | L'impostazione della cella. |

### Valore di ritorno

Restituisce i dati dell'immagine dell'icona.

### Esempi

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



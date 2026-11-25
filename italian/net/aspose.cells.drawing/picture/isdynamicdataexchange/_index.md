---
title: "Picture.IsDynamicDataExchange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene o imposta se lo scambio dinamico di dati"
type: docs
url: /it/net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

Ottiene o imposta se lo scambio dinamico di dati

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsDynamicDataExchangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Dimostra la proprietà IsDynamicDataExchange
            Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
            
            // Imposta IsDynamicDataExchange su true
            picture.IsDynamicDataExchange = true;
            Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);

            // Salva la cartella di lavoro
            workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);

            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
            Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
            Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



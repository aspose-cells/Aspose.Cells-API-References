---
title: "Picture.IsAutoSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. True indica che la dimensione dell'oggetto ole verrà modificata automaticamente in base alla dimensione dell'istantanea del contenuto incorporato quando l'oggetto ole è attivato"
type: docs
url: /it/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

True indica che la dimensione dell'oggetto ole verrà modificata automaticamente in base alla dimensione dell'istantanea del contenuto incorporato quando l'oggetto ole è attivato.

```csharp
public bool IsAutoSize { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Dimostra la proprietà IsAutoSize
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Imposta IsAutoSize su true - l'immagine verrà ridimensionata automaticamente per adattarsi al contenuto
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Imposta IsAutoSize su false - l'immagine manterrà le sue dimensioni originali
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Salva la cartella di lavoro
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



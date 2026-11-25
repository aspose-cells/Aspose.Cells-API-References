---
title: "MsoFillFormatHelper.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Ottiene e imposta i dati di riempimento Texture e Picture"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/imagedata/
---
## MsoFillFormatHelper.ImageData property

Ottiene e imposta i dati di riempimento Texture e Picture.

```csharp
public byte[] ImageData { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "ImageData Property Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visualizza il valore corrente della proprietà ImageData
                Console.WriteLine($"Current ImageData: {(fillHelper.ImageData == null ? "null" : $"Length: {fillHelper.ImageData.Length} bytes")}");

                // Imposta nuovi dati immagine (crea una semplice immagine rossa 1x1 pixel)
                byte[] imageData = new byte[] { 0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00, 0x28, 0x00,
                                               0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00, 0x00 };

                fillHelper.ImageData = imageData;
                Console.WriteLine($"Updated ImageData length: {fillHelper.ImageData.Length} bytes");

                // Dimostra la lettura del valore di ImageData
                byte[] currentImageData = fillHelper.ImageData;
                Console.WriteLine($"Current ImageData length: {currentImageData.Length} bytes");

                // Salva la cartella di lavoro per dimostrare l'esecuzione corretta
                workbook.Save("ImageDataDemo.xlsx");

                Console.WriteLine("ImageData property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ImageData demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



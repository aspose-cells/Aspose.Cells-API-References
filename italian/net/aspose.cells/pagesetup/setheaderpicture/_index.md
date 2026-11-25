---
title: "PageSetup.SetHeaderPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta un'immagine nell'intestazione di un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Imposta un'immagine nell'intestazione di un foglio di lavoro.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerPicture | Byte[] | Dati immagine. |

### Valore di ritorno

Restituisce l'oggetto [`Picture`](../../../aspose.cells.drawing/picture/) .

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Carica un file immagine in un array di byte
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Chiama SetHeaderPicture con l'indice della sezione (0 per l'intestazione centrale) e i byte dell'immagine
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Imposta lo script dell'intestazione per visualizzare l'immagine
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



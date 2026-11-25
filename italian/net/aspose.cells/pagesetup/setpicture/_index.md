---
title: "PageSetup.SetPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta un'immagine nell'intestazione/piè di pagina di un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Imposta un'immagine nell'intestazione/piè di pagina di un foglio di lavoro.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFirst | Booleano | Indica se si sta impostando l'immagine dell'intestazione/piè di pagina della prima pagina. |
| isEven | Booleano | Indica se si sta impostando l'immagine dell'intestazione/piè di pagina delle pagine pari. |
| isHeader | Booleano | Indica se si sta impostando l'immagine dell'intestazione/piè di pagina. |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| imageData | Byte[] | Dati immagine. |

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

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Carica un file immagine in un array di byte
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Chiama il metodo SetPicture per impostare l'immagine dell'intestazione
                // Parametri: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Imposta il testo dell'intestazione
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Salva la cartella di lavoro
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



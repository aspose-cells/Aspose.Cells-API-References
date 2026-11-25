---
title: "PageSetup.SetFooterPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta un'immagine nel piè di pagina di un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Imposta un'immagine nel piè di pagina di un foglio di lavoro.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerPicture | Byte[] | Dati immagine. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Carica un file immagine in un array di byte
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Chiama il metodo SetFooterPicture con l'indice della sezione (0 per centro, 1 per sinistra, 2 per destra) e i dati dell'immagine
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Imposta il testo del piè di pagina da visualizzare insieme all'immagine
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Salva la cartella di lavoro per vedere l'immagine del piè di pagina
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
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



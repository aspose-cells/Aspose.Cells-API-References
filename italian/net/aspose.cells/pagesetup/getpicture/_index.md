---
title: "PageSetup.GetPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Ottiene l'oggetto Picture dell'intestazione / piè di pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Ottiene l'oggetto [`Picture`](../../../aspose.cells.drawing/picture/) dell'intestazione / piè di pagina.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isHeader | Booleano | Indica se si trova nell'intestazione o nel piè di pagina. |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

### Valore di ritorno

Restituisce l'oggetto [`Picture`](../../../aspose.cells.drawing/picture/). Restituisce null se non c'è alcuna immagine.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine all'intestazione del foglio di lavoro
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Ottieni l'immagine dall'intestazione e modifica la sua luminosità
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Ottiene l'oggetto [`Picture`](../../../aspose.cells.drawing/picture/) dell'intestazione / piè di pagina.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFirst | Booleano | Indica se si sta ottenendo l'immagine dell'intestazione/piè di pagina della prima pagina. |
| isEven | Booleano | Indica se si sta ottenendo l'immagine dell'intestazione/piè di pagina delle pagine pari. |
| isHeader | Booleano | Indica se si sta ottenendo l'immagine dell'intestazione/piè di pagina. |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |

### Valore di ritorno

Restituisce l'oggetto [`Picture`](../../../aspose.cells.drawing/picture/) .

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni l'oggetto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta alcune proprietà di intestazione/piè di pagina per garantire che ci siano immagini da recuperare
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Chiama il metodo GetPicture con i parametri: isFirst, isEven, isHeader, section
                // Verifica l'intestazione della prima pagina (sezione 0 - intestazione centrale)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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



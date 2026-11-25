---
title: "PageSetup.SetHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta uno script che formatta l'intestazione di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Imposta uno script per formattare l'intestazione di un file Excel.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| headerScript | String | Script di formattazione dell'intestazione. |

### Osservazioni

Comandi script:

| **Command** | **Description** |
| --- | --- |
| &amp;P | Numero di pagina corrente |
| &amp;N | Conteggio pagine |
| &amp;D | Data corrente |
| &amp;T | Ora corrente |
| &amp;A | Nome del foglio |
| &amp;F | Nome file senza percorso |
| &amp;\"&lt;FontName&gt;\" | Nome del font, ad esempio: &amp;\"Arial\" |
| &amp;\"&lt;FontName&gt;, &lt;FontStyle&gt;\" | Nome del font e stile del font, ad esempio: &amp;\"Arial,Bold\" |
| &amp;&lt;FontSize&gt; | Dimensione del carattere. Se questo comando è seguito da un numero semplice da stampare nell'intestazione, sarà separato dall'altezza del carattere da uno spazio. |
| &amp;K&lt;RRGGBB&gt; | Colore del carattere, ad esempio (ROSSO): &amp;KFF0000 |
| &amp;G | Script immagine |

Ad esempio: "&amp;Arial,Bold&amp;8Header Note"

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta diverse sezioni dell'intestazione con vari comandi
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



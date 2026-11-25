---
title: "PageSetup.SetFooter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PageSetup. Imposta uno script che formatta il piè di pagina di un file Excel"
type: docs
url: /it/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Imposta uno script per formattare il piè di pagina di un file Excel.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| section | Int32 | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra. |
| footerScript | String | Script di formattazione del piè di pagina. |

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

Ad esempio: "&amp;Arial,Bold&amp;8Footer Note"

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



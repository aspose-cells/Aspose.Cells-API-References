---
title: "Hyperlink.ScreenTip"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Hyperlink. Restituisce o imposta il testo ScreenTip per l'hyperlink specificato"
type: docs
url: /it/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Restituisce o imposta il testo ScreenTip per il collegamento ipertestuale specificato.

```csharp
public string ScreenTip { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Crea un hyperlink con ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Salva la cartella di lavoro
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



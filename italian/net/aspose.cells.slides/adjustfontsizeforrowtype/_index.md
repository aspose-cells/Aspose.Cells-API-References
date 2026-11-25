---
title: "Enum AdjustFontSizeForRowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Rappresenta quale tipo di righe dovrebbe essere regolato"
type: docs
url: /it/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Rappresenta quali tipi di righe devono essere aggiustate.

```csharp
public enum AdjustFontSizeForRowType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna regolazione. |
| EmptyRows | `1` | Se la riga è vuota, cambia la dimensione del carattere per adattarla all'altezza della riga. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crea un'istanza di PptxSaveOptions con l'impostazione AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Salva la cartella di lavoro come file PPTX
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)



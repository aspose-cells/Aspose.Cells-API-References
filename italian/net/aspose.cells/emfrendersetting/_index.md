---
title: "Enum EmfRenderSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.EmfRenderSetting. Impostazione per il rendering del metafile Emf"
type: docs
url: /it/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Impostazione per il rendering del metafile Emf.

```csharp
public enum EmfRenderSetting
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| EmfOnly | `0` | Solo rendering dei record Emf. |
| EmfPlusPrefer | `1` | Preferisci il rendering dei record EmfPlus. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Crea opzioni immagine con impostazione di rendering EMF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Crea un rendering del foglio con le opzioni
            SheetRender render = new SheetRender(worksheet, options);

            // Salva la prima pagina come immagine EMF
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



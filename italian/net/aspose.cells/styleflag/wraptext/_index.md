---
title: "StyleFlag.WrapText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione di avvolgimento del testo"
type: docs
url: /it/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

L'impostazione di a capo automatico sarà applicata.

```csharp
public bool WrapText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con avvolgimento del testo abilitato
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Crea un flag di stile e abilita il flag WrapText
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Applica lo stile alla cella A1 con i flag specificati
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Adatta automaticamente l'altezza della riga per vedere il testo avvolto
            worksheet.AutoFitRow(0);

            // Salva la cartella di lavoro
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



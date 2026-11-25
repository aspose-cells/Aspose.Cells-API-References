---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ottiene e imposta il tipo di adattamento automatico dell'altezza della riga per le celle unite"
type: docs
url: /it/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Ottiene e imposta il tipo di adattamento automatico dell'altezza della riga per le celle unite.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Osservazioni

Excel, per impostazione predefinita, ignora le celle unite quando adatta l'altezza della riga, quindi Aspose.Cells funziona come il valore predefinito di MS Excel. Si prega di impostare questo tipo per modificare il modo di adattamento automatico dell'altezza della riga delle celle unite.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio e unisci le celle
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // Adatta automaticamente le righe con AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Adatta automaticamente le colonne con AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Salva la cartella di lavoro
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



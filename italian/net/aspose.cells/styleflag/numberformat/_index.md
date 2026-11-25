---
title: "StyleFlag.NumberFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione del formato numerico verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

L'impostazione del formato numerico sarà applicata.

```csharp
public bool NumberFormat { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Imposta valore della cella
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Crea stile di formato numerico personalizzato
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Applica solo il formato numerico usando StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Applica lo stile all'intervallo di celle (qualifica completamente il tipo Range)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Salva e verifica
            workbook.Save("output_number_format.ods");
            
            // Ricarica per verificare
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



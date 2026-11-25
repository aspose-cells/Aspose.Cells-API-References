---
title: "UnionRange.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Copia l'intervallo con opzioni di incolla speciale"
type: docs
url: /it/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Copia l'intervallo con le opzioni incolla speciale.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | UnionRange | L'intervallo di origine. |
| opzioni | PasteOptions | Le opzioni Incolla speciale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Crea UnionRange di origine
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Crea UnionRange di destinazione
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Crea PasteOptions con impostazioni specifiche
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Chiama il metodo Copy
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Salva la cartella di lavoro
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



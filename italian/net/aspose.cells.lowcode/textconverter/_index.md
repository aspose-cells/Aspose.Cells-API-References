---
title: "Classe TextConverter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.LowCode.TextConverter class. Convertitore per la conversione tra formati basati su testo csv tsv dif... e altri formati di file di foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

Convertitore per la conversione tra formati basati su testo (csv, tsv, dif…) e altri formati di file di foglio di calcolo.

```csharp
public class TextConverter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converte il formato del file tra formati basati su testo e altri formati di foglio di calcolo |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Converte il file modello fornito tra file basati su testo e altri formati. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterDemo
    {
        public static void Process(string inputFile, string outputFile)
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            string[] lines = File.ReadAllLines(inputFile);
            for (int i = 0; i < lines.Length; i++)
            {
                string[] cells = lines[i].Split(',');
                for (int j = 0; j < cells.Length; j++)
                {
                    worksheet.Cells[i, j].PutValue(cells[j]);
                }
            }

            workbook.Save(outputFile, SaveFormat.Xlsx);
        }
    }

    public class LowCodeClassTextConverterDemo
    {
        public static void Run()
        {
            TextConverter.Process("template.csv", "res.xlsx");
            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



---
title: "Klass TextConverter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.TextConverter-klass. Konverterare för konvertering mellan textbaserade format csv tsv dif... och andra kalkylbladsfilformat"
type: docs
url: /sv/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

Konverterare för konvertering mellan textbaserade format (csv, tsv, dif…) och andra kalkylbladsfilformat.

```csharp
public class TextConverter
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konverterar filformat mellan textbaserade format och andra kalkylbladsfilformat |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Konverterar given mallfil mellan textbaserade filer och andra format. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



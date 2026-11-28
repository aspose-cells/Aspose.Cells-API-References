---
title: "Sınıf TextConverter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.TextConverter sınıfı. Metin tabanlı formatlar (csv, tsv, dif...) ve diğer elektronik tablo dosya formatları arasında dönüşüm yapan dönüştürücü"
type: docs
url: /tr/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

Metin tabanlı formatlar (csv, tsv, dif...) ile diğer elektronik tablo dosya formatları arasında dönüşüm için dönüştürücü.

```csharp
public class TextConverter
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Metin tabanlı formatlar ile diğer elektronik tablo dosya formatları arasında dosya formatını dönüştürür |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Verilen şablon dosyasını metin tabanlı dosyalar ile diğer formatlar arasında dönüştürür. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



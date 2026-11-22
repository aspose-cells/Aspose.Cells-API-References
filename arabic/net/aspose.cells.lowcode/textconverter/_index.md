---
title: "Class TextConverter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.LowCode.TextConverter class. محول للتحويل بين صيغ النص مثل csv, tsv, dif... وغيرها من صيغ ملفات الجداول"
type: docs
url: /ar/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

محول للتحويل بين الصيغ النصية (csv، tsv، dif...) وصيغ ملفات جداول البيانات الأخرى.

```csharp
public class TextConverter
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | يقوم بتحويل تنسيق الملف بين الصيغ النصية وصيغ ملفات الجداول الأخرى |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | يقوم بتحويل ملف القالب المحدد بين الملفات النصية والصيغ الأخرى. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



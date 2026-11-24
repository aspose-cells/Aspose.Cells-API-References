---
title: "Klasse TextConverter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.TextConverter class. Konverter für die Umwandlung zwischen textbasierten Formaten csv, tsv, dif... und anderen Tabellenkalkulationsdateiformaten"
type: docs
url: /de/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

Konverter für die Umwandlung zwischen textbasierten Formaten (csv, tsv, dif…) und anderen Tabellenkalkulationsdateiformaten.

```csharp
public class TextConverter
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konvertiert das Dateiformat zwischen textbasierten Formaten und anderen Tabellenkalkulationsdateiformaten |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Konvertiert die angegebene Vorlagendatei zwischen textbasierten Dateien und anderen Formaten. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



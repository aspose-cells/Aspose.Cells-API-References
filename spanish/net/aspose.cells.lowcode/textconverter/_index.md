---
title: "Clase TextConverter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.LowCode.TextConverter class. Convertidor para la conversión entre formatos basados en texto csv tsv dif... y otros formatos de archivo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

Convertidor para la conversión entre formatos basados en texto (csv, tsv, dif...) y otros formatos de archivos de hoja de cálculo.

```csharp
public class TextConverter
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Convierte el formato de archivo entre formatos basados en texto y otros formatos de archivo de hoja de cálculo |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Convierte el archivo de plantilla dado entre archivos basados en texto y otros formatos. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



---
title: "FileFormatUtil.LoadFormatToSaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Konverterar ett LoadFormat‑värde till ett SaveFormat‑värde om möjligt"
type: docs
url: /sv/net/aspose.cells/fileformatutil/loadformattosaveformat/
---
## FileFormatUtil.LoadFormatToSaveFormat method

Konverterar ett LoadFormat‑värde till ett SaveFormat‑värde om möjligt.

```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Läsformatet. |

### Returvärde

Sparaformatet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatUtilMethodLoadFormatToSaveFormatWithLoadFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                LoadFormat inputFormat = LoadFormat.Xlsx;

                SaveFormat outputFormat = FileFormatUtil.LoadFormatToSaveFormat(inputFormat);
                Console.WriteLine($"Converted LoadFormat.{inputFormat} to SaveFormat.{outputFormat}");

                string fileExtension = FileFormatUtil.SaveFormatToExtension(outputFormat);
                string outputFileName = $"OutputFile_{DateTime.Now.Ticks}.{fileExtension}";
                
                workbook.Save(outputFileName, outputFormat);
                Console.WriteLine($"Workbook saved successfully as: {outputFileName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion or saving: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



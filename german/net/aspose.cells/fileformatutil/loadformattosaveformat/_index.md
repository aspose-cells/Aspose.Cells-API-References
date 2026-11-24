---
title: "FileFormatUtil.LoadFormatToSaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Konvertiert einen LoadFormat-Wert in einen SaveFormat-Wert, falls möglich"
type: docs
url: /de/net/aspose.cells/fileformatutil/loadformattosaveformat/
---
## FileFormatUtil.LoadFormatToSaveFormat method

Konvertiert einen LoadFormat-Wert, falls möglich, in einen SaveFormat-Wert.

```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | LoadFormat | Das Ladeformat. |

### Rückgabewert

Das Speicherformat.

### Beispiele

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

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



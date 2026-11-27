---
title: "FileFormatUtil.IsTemplateFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Returnerar true om filändelsen är .xlt .xltX .xltm.ots"
type: docs
url: /sv/net/aspose.cells/fileformatutil/istemplateformat/
---
## FileFormatUtil.IsTemplateFormat method

Returnerar true om ändelsen är .xlt, .xltX, .xltm, .ots.

```csharp
public static bool IsTemplateFormat(string extension)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filändelse | String |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatUtilMethodIsTemplateFormatWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            string extension = ".xltx";

            try
            {
                bool isTemplate = FileFormatUtil.IsTemplateFormat(extension);
                Console.WriteLine($"Is '{extension}' a template format? {isTemplate}");

                if (isTemplate)
                {
                    SaveFormat saveFormat = FileFormatUtil.ExtensionToSaveFormat(extension);
                    workbook.Save($"IsTemplateFormatDemo{extension}", saveFormat);
                    Console.WriteLine($"Workbook saved as template format: {extension}");
                }
            }
            catch (ArgumentException argEx)
            {
                Console.WriteLine($"Invalid argument: {argEx.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



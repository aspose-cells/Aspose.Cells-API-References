---
title: "FileFormatUtil.IsTemplateFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Возвращает true, если расширение .xlt .xltX .xltm.ots"
type: docs
url: /ru/net/aspose.cells/fileformatutil/istemplateformat/
---
## FileFormatUtil.IsTemplateFormat method

Возвращает true, если расширение равно .xlt, .xltX, .xltm,.ots.

```csharp
public static bool IsTemplateFormat(string extension)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| расширение | String |  |

### Примеры

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

### См. также

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



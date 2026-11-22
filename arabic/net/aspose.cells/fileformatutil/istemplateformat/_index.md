---
title: "FileFormatUtil.IsTemplateFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. تُعيد true إذا كان الامتداد .xlt .xltX .xltm .ots"
type: docs
url: /ar/net/aspose.cells/fileformatutil/istemplateformat/
---
## FileFormatUtil.IsTemplateFormat method

يرجع true إذا كان الامتداد .xlt أو .xltX أو .xltm أو .ots.

```csharp
public static bool IsTemplateFormat(string extension)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الامتداد | String |  |

### أمثلة

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

### انظر أيضًا

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



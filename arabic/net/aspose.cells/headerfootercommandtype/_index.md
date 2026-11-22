---
title: "التعداد HeaderFooterCommandType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.HeaderFooterCommandType. يمثل نوع الأمر للترويسة والتذييل"
type: docs
url: /ar/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

يمثل نوع الأمر للترويسة والتذييل.

```csharp
public enum HeaderFooterCommandType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Text | `0` | النص. |
| CurrentPage | `1` | رقم الصفحة الحالي |
| Pagecount | `2` | عدد الصفحات |
| CurrentDate | `3` | التاريخ الحالي |
| CurrentTime | `4` | الوقت الحالي |
| SheetName | `5` | اسم الورقة |
| FileName | `6` | اسم الملف بدون المسار |
| FilePath | `7` | مسار الملف بدون اسم الملف |
| Picture | `8` | صورة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // تعيين الترويسة بأنواع أوامر مختلفة
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // استرجاع أوامر الترويسة
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // عرض قيم HeaderFooterCommandType المختلفة
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // التحقق من أنواع الأوامر المحددة
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // حفظ المصنف لعرض تكوين الترويسة
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "فئة HeaderFooterCommand"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.HeaderFooterCommand. تمثل أمر الترويسة/التذييل"
type: docs
url: /ar/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

يمثل أمر الترويسة/التذييل

```csharp
public class HeaderFooterCommand
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | يسترجع الخط لقيمة الأمر. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | يسترجع نص الأمر. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | يسترجع نوع أمر الرأس/التذييل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى PageSetup وتعيين الرأس باستخدام الأوامر
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // احصل على أوامر الرأس
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // عرض أنواع الأوامر والنص
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



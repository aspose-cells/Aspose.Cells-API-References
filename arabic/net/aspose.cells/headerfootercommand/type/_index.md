---
title: "HeaderFooterCommand.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HeaderFooterCommand. يحصل على نوع أمر الرأس/التذييل"
type: docs
url: /ar/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

يسترجع نوع أمر الرأس/التذييل.

```csharp
public HeaderFooterCommandType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين الترويسة بأنواع أوامر مختلفة
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // احصل على أوامر الرأس
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // توضيح استخدام خاصية Type
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### انظر أيضًا

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



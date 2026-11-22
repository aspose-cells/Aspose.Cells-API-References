---
title: "HeaderFooterCommand.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HeaderFooterCommand. يحصل على نص الأمر"
type: docs
url: /ar/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

يسترجع نص الأمر.

```csharp
public string Text { get; }
```

### ملاحظات

صالح فقط لـ HeaderFooterCommandType.Text.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين رأس باستخدام أمر نصي
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // احصل على أوامر الرأس
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // عرض معلومات حول أمر النص
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // احفظ المصنف
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



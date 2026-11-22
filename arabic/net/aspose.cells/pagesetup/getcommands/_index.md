---
title: "PageSetup.GetCommands"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تحصل على جميع أوامر الرأس أو التذييل"
type: docs
url: /ar/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

يحصل على جميع أوامر الرأس أو التذييل.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| headerFooterScript | String | سكريبت الرأس/التذييل |

### قيمة الإرجاع

يعيد جميع أوامر الرأس أو التذييل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين الرأس باستخدام الأوامر
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // احصل على أوامر الرأس
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // عرض أنواع الأوامر والنص
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### انظر أيضًا

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



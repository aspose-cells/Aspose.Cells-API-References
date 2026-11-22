---
title: "IWarningCallback.Warning"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IWarningCallback. يحتاج رد الاتصال الخاص بنا فقط إلى تنفيذ طريقة Warning"
type: docs
url: /ar/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

يحتاج رد الاتصال الخاص بنا فقط إلى تنفيذ طريقة "Warning".

```csharp
public void Warning(WarningInfo warningInfo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| warningInfo | WarningInfo | معلومات التحذير |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackMethodWarningWithWarningInfoDemo : IWarningCallback
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var demo = new IWarningCallbackMethodWarningWithWarningInfoDemo();
            workbook.Settings.WarningCallback = demo;

            try
            {
                Console.WriteLine("Warning callback is set up. Any warnings during operations will be displayed.");
                
                // إظهار التأثير عن طريق الحفظ مع سيناريو تحذير محتمل
                worksheet.Cells["A1"].Formula = "=1/0"; // This may trigger a warning
                workbook.Save("WarningDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning Type: {warningInfo.Type}");
            Console.WriteLine($"Description: {warningInfo.Description}");
            Console.WriteLine($"Corrected Object: {warningInfo.CorrectedObject ?? "null"}");
        }
    }
}
```

### انظر أيضًا

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



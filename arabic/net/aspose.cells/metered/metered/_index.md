---
title: "Metered.Metered"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ Metered. يهيئ نسخة جديدة من هذه الفئة"
type: docs
url: /ar/net/aspose.cells/metered/metered/
---
## Metered constructor

يُنشئ مثيلًا جديدًا لهذه الفئة.

```csharp
public Metered()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء نسخة باستخدام المنشئ
            Metered metered = new Metered();

            // تعيين ترخيص metered
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // إنشاء دفتر عمل بسيط لتوضيح الوظيفة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // احفظ المصنف
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



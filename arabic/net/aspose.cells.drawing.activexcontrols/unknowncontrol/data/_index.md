---
title: "UnknownControl.Data"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnknownControl. تحصل وتضبط البيانات الثنائية للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

يحصل على البيانات الثنائية للعنصر ويضبطها.

```csharp
public override byte[] Data { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء CLSID تجريبي (معرّف غير صالح)
            byte[] dummyClsid = new byte[16];

            // إضافة عنصر تحكم ActiveX غير معروف باستخدام ControlType.Unknown مع جميع المعاملات
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // الوصول إلى مثيل UnknownControl
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // ضبط بيانات العنصر بما في ذلك CLSID عن طريق النسخ إلى المصفوفة الموجودة
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // قراءة وعرض معلومات خاصية Data
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // عرض استمرارية بيانات التحكم في ملف الإخراج
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



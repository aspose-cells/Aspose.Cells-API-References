---
title: "XmlLoadOptions.StartCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlLoadOptions. تحصل وتضبط الخلية البداية"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

يحصل على خلية البداية ويضبطها.

```csharp
public string StartCell { get; set; }
```

### ملاحظات

يعمل فقط عندما لا يكون الملف speadsheetML أو ربط XML بـ Excel.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // تعيين الخلية البداية لاستيراد بيانات XML
            options.StartCell = "B2";

            // تحميل ملف XML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.xml", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إخراج القيمة من الخلية البداية لتوضيح الخاصية
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



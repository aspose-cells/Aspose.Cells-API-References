---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractTextLoadOptions. تشير إلى الإستراتيجية لتطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة النص إلى رقم أو تاريخ/وقت"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

يشير إلى الاستراتيجية لتطبيق النمط على القيم المحللة عند تحويل قيمة النص إلى رقم أو تاريخ/وقت.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين نمط مخصص للعرض
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // تطبيق النمط على خلية
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // إنشاء بيانات CSV
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // إنشاء خيارات تحميل النص مع LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // استيراد بيانات CSV باستخدام خيارات التحميل المحددة
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // احفظ المصنف لعرض النتيجة
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



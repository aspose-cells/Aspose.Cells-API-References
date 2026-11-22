---
title: "Row.CopySettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. نسخ إعدادات الصف مثل النمط والارتفاع والرؤية ... إلخ"
type: docs
url: /ar/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

نسخ إعدادات الصف، مثل النمط، الارتفاع، الظهور، ...إلخ.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | Row | صف المصدر الذي سيتم نسخ إعداداته إلى هذا الصف |
| checkStyle | منطقي | ما إذا كان سيتم فحص وتجميع النمط. لا يُفعَّل إلا ويكون ضروريًا عندما ينتمي كائنان من الصفوف إلى دفتر عمل مختلف وتكون أنماط دفترَي العمل مختلفتين. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء وتنسيق صف المصدر
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // إنشاء صف الهدف
            Row targetRow = worksheet.Cells.Rows[1];
            
            // توضيح CopySettings مع copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // تحقق من أن الإعدادات تم نسخها
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



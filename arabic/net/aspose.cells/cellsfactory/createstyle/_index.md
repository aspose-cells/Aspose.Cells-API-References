---
title: "CellsFactory.CreateStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsFactory. تنشئ نمطًا جديدًا"
type: docs
url: /ar/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

ينشئ نمطًا جديدًا.

```csharp
public Style CreateStyle()
```

### قيمة الإرجاع

تُرجع كائن نمط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء نمط باستخدام CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // تعيين خصائص الحدود للنمط
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // تطبيق النمط على خلية
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



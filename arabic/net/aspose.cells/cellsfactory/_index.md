---
title: "الفئة CellsFactory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellsFactory. أداة لإنشاء كائنات من نموذج Cells"
type: docs
url: /ar/net/aspose.cells/cellsfactory/
---
## CellsFactory class

أداة لإنشاء كائنات فئات نموذج Cells.

```csharp
public class CellsFactory
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CellsFactory](cellsfactory/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | ينشئ نمطًا جديدًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // إنشاء نسخة جديدة من CellsFactory
            CellsFactory factory = new CellsFactory();

            // استخدام المصنع لإنشاء نمط جديد
            Style style = factory.CreateStyle();

            // تخصيص النمط
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // إنشاء مصنف جديد وورقة عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تطبيق النمط على خلية محددة
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // حفظ المصنف إلى ملف
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



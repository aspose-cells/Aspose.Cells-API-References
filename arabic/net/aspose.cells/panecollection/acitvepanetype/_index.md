---
title: "PaneCollection.AcitvePaneType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaneCollection. تحصل وتعيّن الجزء النشط"
type: docs
url: /ar/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

يحصل على ويضبط الجزء النشط.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية [`ActivePaneType`](../activepanetype/). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية لتوضيح تقسيم الجزء
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // تقسيم ورقة العمل إلى أجزاء
            worksheet.Split();

            // الحصول على مجموعة الأجزاء
            PaneCollection panes = worksheet.GetPanes();

            // عرض الجزء النشط الحالي
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // تعيين الجزء النشط إلى BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // تعيين الصف/العمود الأول الظاهر للأجزاء السفلية/اليمنى
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // احفظ المصنف
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



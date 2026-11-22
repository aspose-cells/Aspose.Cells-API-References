---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaneCollection. تحصل وتعيّن العمود الأول الظاهر في الجزء الأيمن"
type: docs
url: /ar/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

يحصل على ويضبط العمود المرئي الأول للجزء الأيمن.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // تجميد الأجزاء عن طريق تحديد مؤشرات الصف والعمود (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // الحصول على مجموعة الأجزاء
            PaneCollection panes = sheet.GetPanes();
            
            // تعيين العمود الأول الظاهر في الجزء الأيمن
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



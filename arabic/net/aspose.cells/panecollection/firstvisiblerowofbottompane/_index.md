---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaneCollection. تحصل وتعيّن الصف الأول الظاهر في الجزء السفلي"
type: docs
url: /ar/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

يحصل على ويضبط الصف المرئي الأول للجزء السفلي.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية لإنشاء جزء قابل للتمرير
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // تجميد الأجزاء عند الصف 10 (سيؤدي ذلك إلى إنشاء أجزاء علوية وسفلية)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // الحصول على مجموعة الأجزاء
            PaneCollection panes = worksheet.GetPanes();
            
            // تعيين الصف الأول الظاهر في الجزء السفلي
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // إخراج الصف الأول الظاهر في الجزء السفلي
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // احفظ المصنف
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



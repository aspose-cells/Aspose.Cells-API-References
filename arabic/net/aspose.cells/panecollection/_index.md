---
title: "الفئة PaneCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.PaneCollection. تمثل جميع كائنات Pane المعروضة في النافذة المحددة"
type: docs
url: /ar/net/aspose.cells/panecollection/
---
## PaneCollection class

يمثل جميع كائنات Pane المعروضة في النافذة المحددة.

```csharp
public class PaneCollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) يحصل على ويضبط الجزء النشط. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | يحصل على ويضبط الجزء النشط. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | يحصل على ويضبط العمود المرئي الأول للجزء الأيمن. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | يحصل على ويضبط الصف المرئي الأول للجزء السفلي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // تجميد الأجزاء عند الصف 5، العمود 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // احصل على مجموعة الأجزاء
            PaneCollection panes = sheet.GetPanes();
            
            // تعديل إعدادات الجزء
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // احفظ المصنف
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



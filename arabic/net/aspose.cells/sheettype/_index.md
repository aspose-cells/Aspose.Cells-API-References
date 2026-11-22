---
title: "تعداد SheetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.SheetType enum. يحدد نوع ورقة العمل"
type: docs
url: /ar/net/aspose.cells/sheettype/
---
## SheetType enumeration

يحدد نوع ورقة العمل.

```csharp
public enum SheetType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| VB | `0` | وحدة Visual Basic |
| Worksheet | `1` |  |
| Chart | `2` | مخطط |
| BIFF4Macro | `3` | ورقة ماكرو BIFF4 |
| InternationalMacro | `4` | ورقة ماكرو دولية |
| Other | `5` |  |
| Dialog | `6` | ورقة عمل حوارية |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إدراج ورقة عمل جديدة من النوع Worksheet في الفهرس 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // تعيين اسم ورقة العمل الجديدة
            newWorksheet.Name = "InsertedSheet";
            
            // الوصول إلى الخلايا في ورقة العمل الجديدة وإضافة بعض البيانات
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // احفظ المصنف
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



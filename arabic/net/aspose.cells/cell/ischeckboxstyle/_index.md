---
title: "Cell.IsCheckBoxStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كان يتم تعيين هذه الخلية كخانة اختيار"
type: docs
url: /ar/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

يشير إلى ما إذا كان يتم تعيين هذه الخلية كمربع اختيار.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية B1 وتعيينها بنمط خانة اختيار
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // الوصول إلى الخلية A1 وتعيينها بنمط خانة اختيار مع قيمة
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // احفظ المصنف
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // تحميل المصنف المحفوظ للتحقق من الخصائص
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // تحقق من أن B1 بنمط خانة اختيار
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // غيّر B1 إلى نمط غير خانة اختيار واحفظ
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



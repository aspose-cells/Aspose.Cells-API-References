---
title: "التعداد CellsUnitType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.CellsUnitType. يحدد وحدة القياس"
type: docs
url: /ar/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

يحدد وحدة القياس.

```csharp
public enum CellsUnitType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Pixel | `1` | القياس بوحدات البكسل. |
| Point | `2` | القياس بوحدات النقاط. النقطة تمثل 1/72 من البوصة. |
| Inch | `4` | القياس بوحدات البوصة. |
| Cm | `6` | القياس بوحدات السنتيمتر. |
| Character | `7` | بوحدة الأحرف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // عرض استخدام قيم مختلفة لتعداد CellsUnitType
                Console.WriteLine("Available CellsUnitType values:");

                // عرض جميع قيم التعداد
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // مثال على الاستخدام: تعيين عرض العمود باستخدام وحدات مختلفة
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // احفظ المصنف لعرض تدفق كامل
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



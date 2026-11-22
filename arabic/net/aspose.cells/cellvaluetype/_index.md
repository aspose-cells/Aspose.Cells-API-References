---
title: "تعداد CellValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CellValueType تعداد. يحدد نوع قيمة الخلية"
type: docs
url: /ar/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

يحدد نوع قيمة الخلية.

```csharp
public enum CellValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| IsUnknown | `0` | نوع قيمة الخلية غير معروف. |
| IsNull | `1` | خلية فارغة. يجب أن تكون القيمة المقابلة null. |
| IsNumeric | `2` | قيمة الخلية رقمية. يجب أن تكون القيمة المقابلة int أو double. |
| IsDateTime | `4` | قيمة الخلية تاريخ/وقت. يجب أن تكون القيمة المقابلة DateTime. |
| IsString | `8` | قيمة الخلية نصية. يجب أن تكون القيمة المقابلة string. |
| IsBool | `16` | قيمة الخلية منطقية. يجب أن تكون القيمة المقابلة bool. |
| IsError | `32` | الخلية تحتوي على قيمة خطأ. يجب أن تكون القيمة المقابلة سلسلة خطأ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // تحقق واعرض أنواع قيم الخلايا
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // احفظ المصنف
            workbook.Save("CellValueTypeExample.xlsx");
            workbook.Save("CellValueTypeExample.pdf");
        }

        private static void DisplayCellValueType(Cell cell)
        {
            Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");

            switch (cell.Type)
            {
                case CellValueType.IsNumeric:
                    Console.WriteLine("The cell contains a numeric value.");
                    break;
                case CellValueType.IsString:
                    Console.WriteLine("The cell contains a string value.");
                    break;
                case CellValueType.IsDateTime:
                    Console.WriteLine("The cell contains a DateTime value.");
                    break;
                case CellValueType.IsBool:
                    Console.WriteLine("The cell contains a boolean value.");
                    break;
                case CellValueType.IsNull:
                    Console.WriteLine("The cell is blank.");
                    break;
                case CellValueType.IsError:
                    Console.WriteLine("The cell contains an error value.");
                    break;
                default:
                    Console.WriteLine("The cell value type is unknown.");
                    break;
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



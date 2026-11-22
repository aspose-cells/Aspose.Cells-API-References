---
title: "Cell.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على اسم الخلية"
type: docs
url: /ar/net/aspose.cells/cell/name/
---
## Cell.Name property

يحصل على اسم الخلية.

```csharp
public string Name { get; }
```

### ملاحظات

يتضمن اسم الخلية حرف العمود ورقم الصف. على سبيل المثال، اسم الخلية في الصف 0 والعمود 0 هو A1.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقات مسماة للخلايا ذات أنواع القيم المختلفة
            worksheet.Cells.CreateRange("A1").Name = "NumericCell";
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(42.5);

            worksheet.Cells.CreateRange("B1").Name = "StringCell";
            Cell cell2 = worksheet.Cells["B1"];
            cell2.PutValue("Hello World");

            worksheet.Cells.CreateRange("C1").Name = "DateTimeCell";
            Cell cell3 = worksheet.Cells["C1"];
            cell3.PutValue(DateTime.Now);

            // عرض معلومات الخلية باستخدام خاصية Name الخاصة بها
            PrintCellInfo(cell1);
            PrintCellInfo(cell2);
            PrintCellInfo(cell3);
        }

        private static void PrintCellInfo(Cell cell)
        {
            Console.WriteLine($"Cell '{cell.Name}' has value: {cell.Value} and type: {cell.Type}");

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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



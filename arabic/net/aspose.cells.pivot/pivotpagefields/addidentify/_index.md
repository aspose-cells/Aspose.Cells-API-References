---
title: "PivotPageFields.AddIdentify"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotPageFields. تحدد أي تسمية عنصر في كل حقل صفحة تُستخدم لتحديد نطاق البيانات. يجب أن يكون طول pageItemIndex مساويًا لـ PageFieldCount لذا يرجى إضافة حقل الصفحة أولاً"
type: docs
url: /ar/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

يضبط أي تسمية عنصر في كل حقل صفحة لاستخدامها لتحديد نطاق البيانات. يجب أن يكون طول pageItemIndex مساويًا لـ PageFieldCount، لذا يرجى إضافة حقل الصفحة أولاً.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeIndex | Int32 | فهرس نطاق بيانات التجميع. |
| pageItemIndex | Int32[] | فهرس عنصر الصفحة في كل حقل صفحة. pageItemIndex[2] = 1 يعني العنصر الثاني في الحقل الثالث يُستخدم لتحديد هذا النطاق. pageItemIndex[1] = -1 يعني عدم وجود عنصر في الحقل الثاني لتحديد هذا النطاق وستقوم MS بإنشاء عنصر "فارغ" تلقائيًا في الحقل الثاني لتحديد هذا النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // أنشئ كائن PivotPageFields مباشرةً بدلاً من الوصول إليه عبر PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



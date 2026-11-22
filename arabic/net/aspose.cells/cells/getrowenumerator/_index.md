---
title: "Cells.GetRowEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على مُعدد الصفوف"
type: docs
url: /ar/net/aspose.cells/cells/getrowenumerator/
---
## Cells.GetRowEnumerator method

يحصل على مُعدد الصفوف.

```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```

### قيمة الإرجاع

مُعدد الصفوف.

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة RowCollection.GetEnumerator(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مايو 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetRowEnumeratorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Row 1 Data");
            worksheet.Cells["A3"].PutValue("Row 3 Data");
            worksheet.Cells["A5"].PutValue("Row 5 Data");

            try
            {
                // احصل على مُعدد الصفوف من مجموعة Cells
                IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
                
                Console.WriteLine("Iterating through rows containing data:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Cell cell = row.GetCellOrNull(0); // Get first cell in row
                    string cellValue = cell != null ? cell.Value.ToString() : "empty";
                    Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



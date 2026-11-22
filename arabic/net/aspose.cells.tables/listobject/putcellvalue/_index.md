---
title: "ListObject.PutCellValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObject. ضع القيمة في الخلية"
type: docs
url: /ar/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

ضع القيمة في الخلية.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في الجدول. |
| columnOffset | Int32 | إزاحة العمود في الجدول. |
| القيمة | Object | قيمة الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // إظهار PutCellValue مع معلمات Int32, Int32, Object
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // احفظ المصنف
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

ضع القيمة في الخلية.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في الجدول. |
| columnOffset | Int32 | إزاحة العمود في الجدول. |
| القيمة | Object | قيمة الخلية. |
| isTotalsRowLabel | منطقي | يشير إلى ما إذا كان ذلك تسمية لصف الإجمالي، يعمل فقط لصف الإجمالي. إذا كان False وكان هذا الصف صف إجمالي، سيتم إدراج صف جديد. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لإنشاء ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // إنشاء ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // استخدم PutCellValue لتحديث خلية (الصف 2، العمود 1) بقيمة جديدة وتوسيع الجدول
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



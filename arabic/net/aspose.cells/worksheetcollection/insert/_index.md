---
title: "WorksheetCollection.Insert"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. إدراج ورقة عمل"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

(**Obsolete.**) حدّث جميع جداول المحور والرسوم البيانية بمصدر المحور.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الورقة |
| sheetType | SheetType | نوع الورقة. |

### قيمة الإرجاع

يعيد ورقة عمل مدخلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

(**Obsolete.**) حدّث جميع جداول المحور والرسوم البيانية بمصدر المحور.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الورقة |
| sheetType | SheetType | نوع الورقة. |
| sheetName | String | اسم الورقة. |

### قيمة الإرجاع

يعيد ورقة عمل مدخلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إدراج ورقة عمل جديدة في الفهرس 0 بالاسم "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // الوصول إلى ورقة العمل المدخلة
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضع بعض البيانات في الخلية A1 من الورقة المدخلة
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // احفظ المصنف
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



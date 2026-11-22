---
title: "WorksheetCollection.SetOleSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تعيين حجم العرض عندما يُستخدم ملف المصنف ككائن Ole"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

يرتب الأسماء المعرفة.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endColumn | Int32 | فهرس العمود النهائي. |

### ملاحظات

عادةً ما تُستخدم هذه الطريقة لضبط حجم العرض في ملف ppt أو ملف doc.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين حجم OLE لأوراق العمل
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من حجم OLE
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



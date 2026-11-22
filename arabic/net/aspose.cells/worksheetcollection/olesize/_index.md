---
title: "WorksheetCollection.OleSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل وتضبط الحجم المعروض عندما يُستخدم ملف Workbook ككائن Ole"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

يحصل على ويضبط الحجم المعروض عندما يُستخدم ملف المصنف ككائن Ole.

```csharp
public object OleSize { get; set; }
```

### ملاحظات

القيمة Null تعني عدم وجود إعداد حجم ole.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // ضبط حجم OLE لمجموعة أوراق العمل
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // الوصول إلى وعرض خصائص حجم OLE
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // احفظ المصنف
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



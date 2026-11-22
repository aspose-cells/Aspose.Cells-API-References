---
title: "Cells.GetColumnWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Cells method. يحصل على عرض العمود"
type: docs
url: /ar/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

يحصل على عرض العمود.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| isOriginal | منطقي | يشير إلى ما إذا كان يتم الحصول على العرض الأصلي. |
| unitType | CellsUnitType |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين عرض العمود للعمود 1 (فهرس يبدأ من 0)
            cells.SetColumnWidth(0, 20);

            // احصل على عرض العمود بوحدات وأنماط مختلفة
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
        }
    }
}
```

### انظر أيضًا

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

يحصل على عرض (بوحدة الأحرف) للعمود المحدد في العرض العادي.

```csharp
public double GetColumnWidth(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

عرض العمود. في جداول البيانات، يُقاس عرض العمود بعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يُعرض في خط النمط العادي.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين عرض العمود لفهرس العمود 255
            cells.SetColumnWidth(255, 20.86);

            // احصل على عرض العمود وعرضه
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



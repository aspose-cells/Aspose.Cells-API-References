---
title: CopyInRange
second_title: Aspose.Cells لمرجع .NET API
description: انسخ الأشكال الموجودة في النطاق إلى النطاق الوجهة .
type: docs
weight: 380
url: /ar/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

انسخ الأشكال الموجودة في النطاق إلى النطاق الوجهة .

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceShapes | ShapeCollection | أشكال المصدر. |
| ca | CellArea | نطاق المصدر. |
| destRow | Int32 | فهرس صف الإرسال للنطاق المُصَدِّر. |
| destColumn | Int32 | عمود الوجهة من نطاق الوجهة. |
| isContained | Boolean | سواء نسخ الأشكال الموجودة في النطاق فقط. إذا كان صحيحًا ، فقم بنسخ الأشكال الموجودة في النطاق فقط. وإلا فإنه يعمل مثل MS Office. |

### أمثلة

```csharp

[C#]
// إضافة شكل
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
CellArea area2 = new CellArea();
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;

//ينسخ
shapes.CopyInRange(shapes, area2, 12, 1, false);

```

### أنظر أيضا

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../shapecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
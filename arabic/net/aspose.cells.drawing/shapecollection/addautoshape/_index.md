---
title: AddAutoShape
second_title: Aspose.Cells لمرجع .NET API
description: إضافة شكل تلقائي إلى ورقة العمل.
type: docs
weight: 40
url: /ar/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

إضافة شكل تلقائي إلى ورقة العمل.

```csharp
public Shape AddAutoShape(AutoShapeType type, int upperLeftRow, int top, int upperLeftColumn, 
    int left, int height, int width)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| type | AutoShapeType | نوع الشكل التلقائي. |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| top | Int32 | يمثل الإزاحة الرأسية للشكل من صفه الأيسر ، بوحدة البكسل. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| left | Int32 | يمثل الإزاحة الأفقية للشكل من عمودها الأيسر ، بوحدة البكسل. |
| height | Int32 | يمثل ارتفاع الشكل بوحدة البكسل. |
| width | Int32 | يمثل عرض الشكل بوحدة البكسل. |

### قيمة الإرجاع

كائن الشكل.

### ملاحظات

لا يمكن أن يكون النوع Chart / Comment / Picture / OleObject / Polygon / DialogBox

### أمثلة

```csharp

[C#]
// يضيف شكلاً تلقائيًا إلى ورقة العمل.
Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
```

### أنظر أيضا

* class [Shape](../../shape)
* enum [AutoShapeType](../../autoshapetype)
* class [ShapeCollection](../../shapecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../shapecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

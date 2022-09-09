---
title: Group
second_title: Aspose.Cells لمرجع .NET API
description: قم بتجميع الأشكال .
type: docs
weight: 410
url: /ar/net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

قم بتجميع الأشكال .

```csharp
public GroupShape Group(Shape[] groupItems)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| groupItems | Shape[] | عناصر المجموعة. |

### قيمة الإرجاع

أعد شكل المجموعة.

### ملاحظات

يجب عدم تجميع الشكل الموجود في المجموعة . يجب أن يكون الشكل في مجموعة الأشكال هذه.

### أمثلة

```csharp

[C#]
// إضافة الشكل الأول
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// أضف الشكل الثاني
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };
GroupShape groupShape = shapes.Group(shapesArr);

```

### أنظر أيضا

* class [GroupShape](../../groupshape)
* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../shapecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
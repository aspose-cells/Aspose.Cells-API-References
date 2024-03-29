---
title: AddGroupBox
second_title: Aspose.Cells لمرجع .NET API
description: يضيف GroupBox إلى ورقة العمل.
type: docs
weight: 110
url: /ar/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

يضيف GroupBox إلى ورقة العمل.

```csharp
public GroupBox AddGroupBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| top | Int32 | يمثل الإزاحة الرأسية لـ GroupBox من صفه الأيسر ، بوحدة البكسل. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| left | Int32 | يمثل الإزاحة الأفقية لـ GroupBox من عمودها الأيسر ، بوحدة البكسل. |
| height | Int32 | يمثل ارتفاع GroupBox بوحدة البكسل. |
| width | Int32 | يمثل عرض GroupBox بوحدة البكسل. |

### قيمة الإرجاع

كائن GroupBox.

### أمثلة

```csharp

[C#]
// إضافة مربع المجموعة
GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);
```

### أنظر أيضا

* class [GroupBox](../../groupbox)
* class [ShapeCollection](../../shapecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../shapecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

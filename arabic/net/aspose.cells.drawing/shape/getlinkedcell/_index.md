---
title: GetLinkedCell
second_title: Aspose.Cells لمرجع .NET API
description: يحصل على النطاق المرتبط بقيمة عنصر التحكم.
type: docs
weight: 1050
url: /ar/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

يحصل على النطاق المرتبط بقيمة عنصر التحكم.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| isR1C1 | Boolean | ما إذا كانت الصيغة تحتاج إلى تنسيقها كـ R1C1. |
| isLocal | Boolean | ما إذا كانت الصيغة تحتاج إلى التنسيق بواسطة الإعدادات المحلية. |

### قيمة الإرجاع

النطاق المرتبط بقيمة عنصر التحكم.

### أمثلة

```csharp

[C#]
// قد تحصل على نتائج مثل "$ A $ 1"
string link = shape.GetLinkedCell(false, false);
```

### أنظر أيضا

* class [Shape](../../shape)
* مساحة الاسم [Aspose.Cells.Drawing](../../shape)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

---
title: AddIdentify
second_title: Aspose.Cells لمرجع .NET API
description: لتعيين تسمية العنصر في كل حقل صفحة لاستخدامها لتحديد نطاق البيانات. يجب أن تكون قيمة pageItemIndex.Length مساوية لـ PageFieldCount  لذا يرجى إضافة حقل الصفحة أولاً.
type: docs
weight: 30
url: /ar/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

لتعيين تسمية العنصر في كل حقل صفحة لاستخدامها لتحديد نطاق البيانات. يجب أن تكون قيمة pageItemIndex.Length مساوية لـ PageFieldCount ، لذا يرجى إضافة حقل الصفحة أولاً.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| rangeIndex | Int32 | مؤشر نطاق بيانات التوحيد. |
| pageItemIndex | Int32[] | فهرس عنصر الصفحة في حقل كل صفحة . pageItemIndex [2] = 1 يعني العنصر الثاني في الحقل الثالث لاستخدامه لتعريف هذا النطاق. pageItemIndex [1] = -1 يعني عدم وجود عنصر في الحقل الثاني لاستخدامه حدد هذا النطاق وسيقوم MS تلقائيًا بإنشاء عنصر "فارغ" في الحقل الثاني لتحديد هذا النطاق. |

### أنظر أيضا

* class [PivotPageFields](../../pivotpagefields)
* مساحة الاسم [Aspose.Cells.Pivot](../../pivotpagefields)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

---
title: StartCell
second_title: Aspose.Cells لمرجع .NET API
description: يستعد لمعالجة خلية.
type: docs
weight: 30
url: /ar/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

يستعد لمعالجة خلية.

```csharp
public bool StartCell(int columnIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود للخلية المراد معالجتها |

### قيمة الإرجاع

ما إذا كانت هذه الخلية بحاجة إلى المعالجة. خطأ لتجاهل الخلية والتحقق من الخلية التالية حتى تصل إلى نهاية بيانات الخلايا للصف الحالي

### ملاحظات

سيتم استدعاؤها عند الوصول إلى خلية موجودة في الصف الحالي. الصف الحالي هو صف آخر مكالمة لـ[`ProcessRow`](../processrow) .

### أنظر أيضا

* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* مساحة الاسم [Aspose.Cells](../../lightcellsdatahandler)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

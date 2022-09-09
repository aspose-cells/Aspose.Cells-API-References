---
title: GetEnumerator
second_title: Aspose.Cells لمرجع .NET API
description: الحصول على تعداد الخلايا .
type: docs
weight: 720
url: /ar/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

الحصول على تعداد الخلايا .

```csharp
public IEnumerator GetEnumerator()
```

### قيمة الإرجاع

عداد الخلايا

### ملاحظات

عند اجتياز العناصر بواسطة العداد الذي تم إرجاعه ، يجب عدم تعديل مجموعة الخلايا collection (مثل العمليات التي ستتسبب في إنشاء مثيل للخلية / الصف الجديد أو حذف الخلية / الصف الحالي) . وإلا فقد لا يتمكن العداد من اجتياز جميع الخلايا بشكل صحيح (قد يتم اجتياز بعض العناصر بشكل متكرر أو تخطيها).

### أمثلة

```csharp
[C#]
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.Worksheets[0].Cells;

IEnumerator en = cells.GetEnumerator();
while (en.MoveNext())
{
    Cell cell = (Cell)en.Current;
    Console.WriteLine(cell.Name + ": " + cell.Value);
}
```

### أنظر أيضا

* class [Cells](../../cells)
* مساحة الاسم [Aspose.Cells](../../cells)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
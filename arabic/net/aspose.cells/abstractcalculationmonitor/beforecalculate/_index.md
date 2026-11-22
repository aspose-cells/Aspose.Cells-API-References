---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractCalculationMonitor. نفّذ هذه الطريقة للقيام بالعمليات قبل حساب خلية واحدة."
type: docs
url: /ar/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

نفّذ هذه الطريقة للقيام بالمعالجة قبل حساب خلية واحدة.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة التي تنتمي إليها الخلية. |
| rowIndex | Int32 | فهرس الصف للخلية |
| colIndex | Int32 | فهرس العمود للخلية |

### ملاحظات

بالنسبة للخلايا في صيغ المصفوفة، قد لا يتم تنفيذ هذه الطريقة لأن هذه الخلايا عادةً تُحسب معًا.

### انظر أيضًا

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



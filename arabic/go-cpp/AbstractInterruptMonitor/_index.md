---
title: "AbstractInterruptMonitor فئة"
linktitle: "AbstractInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة AbstractInterruptMonitor. تغلف الكائن الذي يمثل abstractinterruptmonitor في Go."
type: docs
weight: 200
url: /ar/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

راقب طلبات الإيقاف في جميع العمليات المستهلكة للوقت.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | عند انقطاع الإجراء، سواءً تم إنهاؤه بهدوء أو رمي استثناء. القيمة الافتراضية هي false، أي عندما تكون IsInterruptionRequested true، سيتم رمي CellsException برمز ExceptionType.Interrupted. |

---
title: "SystemTimeInterruptMonitor فئة"
linktitle: "SystemTimeInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "SystemTimeInterruptMonitor فئة. يغلف الكائن الذي يمثل systemtimeinterruptmonitor في لغة Go."
type: docs
weight: 200
url: /ar/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

تنفيذ بسيط لـ <see cref="AbstractInterruptMonitor"/> عن طريق فحص ومقارنة الوقت الحالي للنظام مع الحد المحدد من قبل المستخدم.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | ينشئ مراقب انقطاع واحد. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [StartMonitor](./startmonitor/) | يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو لحظة استدعاء هذه الطريقة، لذا يجب بدء العملية التي تحتاج إلى مراقبتها مباشرةً بعد هذا الاستدعاء. |
| [IsInterruptionRequested](./isinterruptionrequested/) | يتحقق هذا التنفيذ فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | انظر AbstractInterruptMonitor.TerminateWithoutException. يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء مثيل هذا المراقب. |

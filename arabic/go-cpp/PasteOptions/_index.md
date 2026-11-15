---
title: "فئة PasteOptions"
linktitle: "PasteOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PasteOptions. تغلف الكائن الذي يمثل pasteoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/pasteoptions/
---

## PasteOptions class

يمثل خيارات اللصق الخاص.

```go

type PasteOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPasteOptions](./newpasteoptions/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPasteType](./getpastetype/) | نوع اللصق الخاص. |
| [SetPasteType](./setpastetype/) | نوع اللصق الخاص. |
| [GetShiftFormulasOfShapes](./getshiftformulasofshapes/) | يشير إلى ما إذا كان يجب إزاحة صيغ الأشكال عند نسخ النطاقات. |
| [SetShiftFormulasOfShapes](./setshiftformulasofshapes/) | يشير إلى ما إذا كان يجب إزاحة صيغ الأشكال عند نسخ النطاقات. |
| [GetSkipBlanks](./getskipblanks/) | يشير إلى ما إذا كان يتخطى الخلايا الفارغة. |
| [SetSkipBlanks](./setskipblanks/) | يشير إلى ما إذا كان يتخطى الخلايا الفارغة. |
| [GetKeepOldTables](./getkeepoldtables/) | يحافظ على الجداول في النطاق الوجهة. |
| [SetKeepOldTables](./setkeepoldtables/) | يحافظ على الجداول في النطاق الوجهة. |
| [GetOnlyVisibleCells](./getonlyvisiblecells/) | True يعني نسخ الخلايا المرئية فقط. |
| [SetOnlyVisibleCells](./setonlyvisiblecells/) | True يعني نسخ الخلايا المرئية فقط. |
| [GetTranspose](./gettranspose/) | True لعكس الصفوف والأعمدة عند لصق النطاق. القيمة الافتراضية هي False. |
| [SetTranspose](./settranspose/) | True لعكس الصفوف والأعمدة عند لصق النطاق. القيمة الافتراضية هي False. |
| [GetOperationType](./getoperationtype/) | يحصل على ويضبط نوع العملية عند لصق النطاق. |
| [SetOperationType](./setoperationtype/) | يحصل على ويضبط نوع العملية عند لصق النطاق. |
| [GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | تجاهل الروابط إلى الملف الأصلي. |
| [SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | تجاهل الروابط إلى الملف الأصلي. |

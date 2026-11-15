---
title: "تعداد EquationNodeType"
linktitle: "EquationNodeType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "تعداد EquationNodeType. يحتوي على الكائن الذي يمثل equationnodetype في Go."
type: docs
weight: 200
url: /ar/go-cpp/equationnodetype/
---

## EquationNodeType Enum

نوع عقدة المعادلة. ملاحظة:(1)[1-99] حالياً هناك عقدة واحدة فقط في النطاق، وقيمة تعدادها هي 1. العقدة التي يحددها تُستخدم لتخزين النص الرياضي.(2)[100-199] تشير إلى أن العقدة مكوّن لبعض عقد الدوال الخاصة.(3)[200-] تشير إلى أن العقدة لها بعض الدوال الخاصة.

```go

type EquationNodeType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [UnKnow](./unknow/) | غير معروف |
| [Text](./text/) | يحدد عقدة تخزن نصًا رياضيًا |
| [Base](./base/) | يحدد مكوّن أساسي |
| [Denominator](./denominator/) | يحدد مكوّن مقام |
| [Numerator](./numerator/) | يحدد مكوّن بسط |
| [FunctionName](./functionname/) | يحدد مكوّن اسم الدالة |
| [Subscript](./subscript/) | يحدد مكوّن مؤشر سفلي |
| [Superscript](./superscript/) | يحدد مكوّن مؤشر علوي |
| [Degree](./degree/) | يحدد مكوّن درجة |
| [MatrixRow](./matrixrow/) | يحدد مكوّن صف المصفوفة. صف واحد من المصفوفة |
| [Limit](./limit/) | يمثل كائنًا فرعيًا لدالة الحد الأدنى أو دالة الحد الأعلى |
| [EquationParagraph](./equationparagraph/) | يحدد فقرة رياضية (oMathPara). |
| [LowerLimit](./lowerlimit/) | يحدد دالة الحد الأدنى |
| [UpperLimit](./upperlimit/) | يحدد دالة الحد الأعلى |
| [Mathematical](./mathematical/) | يحدد معادلة أو تعبير رياضي (OMath). |
| [Fraction](./fraction/) | يحدد معادلة كسرية |
| [Function](./function/) | يحدد معادلة دالة |
| [Delimiter](./delimiter/) | يحدد معادلة محدد |
| [Nary](./nary/) | يحدد معادلة عامل متعدد المتغيرات |
| [Radical](./radical/) | يحدد معادلة الجذر |
| [Sup](./sup/) | يحدد معادلة مؤشر علوي |
| [Sub](./sub/) | يحدد معادلة سفلية |
| [SubSup](./subsup/) | يحدد معادلة ذات أسس وفواصل سفلية إلى يمين المعاملات. |
| [PreSubSup](./presubsup/) | يحدد معادلة ذات أسس وفواصل سفلية إلى يسار المعاملات. |
| [Accent](./accent/) | يحدد معادلة لهجة |
| [Bar](./bar/) | يحدد معادلة شريطية |
| [BorderBox](./borderbox/) | يحدد معادلة صندوق الحدود |
| [Box](./box/) | يحدد معادلة صندوق |
| [GroupChr](./groupchr/) | يحدد معادلة مجموعة-حرف |
| [Matrix](./matrix/) | يحدد معادلة المصفوفة، |
| [ArrayEquation](./arrayequation/) | يحدد دالة مصفوفة المعادلات. الدالة تتكون من معادلة واحدة أو أكثر. |

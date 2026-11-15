---
title: "فئة EquationNodeParagraph"
linktitle: "EquationNodeParagraph"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة EquationNodeParagraph. تغلف الكائن الذي يمثل equationnodeparagraph في Go."
type: docs
weight: 200
url: /ar/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

هذه الفئة تحدد فقرة رياضية تحتوي على عنصر واحد أو أكثر من MathEquationNode(OMath).

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetJustification](./getjustification/) | يحدد هذا محاذاة الفقرة الرياضية (سلسلة من المعادلات المتجاورة داخل نفس الفقرة). يمكن أن تكون الفقرة الرياضية محاذاة إلى اليسار، أو إلى اليمين، أو في الوسط، أو في الوسط كمجموعة. بشكل افتراضي، تكون الفقرة الرياضية في الوسط كمجموعة. هذا يعني أن المعادلات يمكن أن تُمحاذَة بالنسبة لبعضها البعض، لكن مجموعة المعادلات بأكملها تكون في الوسط ككل. |
| [SetJustification](./setjustification/) | يحدد هذا محاذاة الفقرة الرياضية (سلسلة من المعادلات المتجاورة داخل نفس الفقرة). يمكن أن تكون الفقرة الرياضية محاذاة إلى اليسار، أو إلى اليمين، أو في الوسط، أو في الوسط كمجموعة. بشكل افتراضي، تكون الفقرة الرياضية في الوسط كمجموعة. هذا يعني أن المعادلات يمكن أن تُمحاذَة بالنسبة لبعضها البعض، لكن مجموعة المعادلات بأكملها تكون في الوسط ككل. |
| [Equals](./equals/) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [GetStartIndex](./getstartindex/) | يحصل على فهرس البداية للأحرف. |
| [GetLength](./getlength/) | يحصل على طول الأحرف. |
| [GetFont](./getfont/) | يعيد الخط لهذا الكائن. |
| [SetWordArtStyle](./setwordartstyle/) | يضبط نمط WordArt المسبق. |
| [GetTextOptions](./gettextoptions/) | يعيد خيارات النص. |
| [GetType](./gettype/) | يحصل على نوع عقدة النص. |
| [GetParentNode](./getparentnode/) | يحدد العقدة الأم للعقدة الحالية |
| [SetParentNode](./setparentnode/) | يحدد العقدة الأم للعقدة الحالية |
| [ToLaTeX](./tolatex/) | حوّل هذه المعادلة إلى تعبير LaTeX. |
| [ToMathML](./tomathml/) | حوّل هذه المعادلة إلى تعبير MathML. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | أدرج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [InsertChild](./insertchild/) | يدرج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية. |
| [InsertAfter](./insertafter/) | يدرج العقدة المحددة بعد العقدة الحالية. |
| [InsertBefore](./insertbefore/) | يدرج العقدة المحددة قبل العقدة الحالية. |
| [GetChild](./getchild/) | يعيد العقدة الموجودة في الفهرس المحدد بين أبناء العقدة الحالية. |
| [Remove](./remove/) | يزيل نفسه من العنصر الأب. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | يزيل العقدة المحددة من أبناء العقدة الحالية. |
| [RemoveAllChildren](./removeallchildren/) | يزيل جميع العقد الفرعية للعقدة الحالية. |
| [GetEquationType](./getequationtype/) | احصل على نوع المعادلة للعقدة الحالية |
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | أنشئ عقدة من النوع المحدد. |

---
title: "فئة EquationNode"
linktitle: "EquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة EquationNode. تغلف الكائن الذي يمثل equationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/equationnode/
---

## EquationNode class

فئة مجردة لاشتقاق عقد معادلات أخرى.

```go

type EquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewEquationNode](./newequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetParentNode](./getparentnode/) | يحدد العقدة الأم للعقدة الحالية |
| [SetParentNode](./setparentnode/) | يحدد العقدة الأم للعقدة الحالية |
| [ToLaTeX](./tolatex/) | حوّل هذه المعادلة إلى تعبير LaTeX. |
| [ToMathML](./tomathml/) | حوّل هذه المعادلة إلى تعبير MathML. |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | أدرج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [AddChild_EquationNode](./addchild_equationnode/) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية. |
| [InsertChild](./insertchild/) | يدرج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية. |
| [InsertAfter](./insertafter/) | يدرج العقدة المحددة بعد العقدة الحالية. |
| [InsertBefore](./insertbefore/) | يدرج العقدة المحددة قبل العقدة الحالية. |
| [GetChild](./getchild/) | يعيد العقدة الموجودة في الفهرس المحدد بين أبناء العقدة الحالية. |
| [Remove](./remove/) | يزيل نفسه من العنصر الأب. |
| [RemoveChild_EquationNode](./removechild_equationnode/) | يزيل العقدة المحددة من أبناء العقدة الحالية. |
| [RemoveChild_Int](./removechild_int/) | يزيل العقدة الموجودة في الفهرس المحدد من أبناء العقدة الحالية. |
| [RemoveAllChildren](./removeallchildren/) | يزيل جميع العقد الفرعية للعقدة الحالية. |
| [Equals](./equals/) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [GetType](./gettype/) | يمثل نوع العقدة. |
| [GetEquationType](./getequationtype/) | احصل على نوع المعادلة للعقدة الحالية |
| [EquationNode_CreateNode](./equationnode_createnode/) | أنشئ عقدة من النوع المحدد. |
| [GetStartIndex](./getstartindex/) | يحصل على فهرس البداية للأحرف. |
| [GetLength](./getlength/) | يحصل على طول الأحرف. |
| [GetFont](./getfont/) | يعيد الخط لهذا الكائن. |
| [SetWordArtStyle](./setwordartstyle/) | يضبط نمط WordArt المسبق. |
| [GetTextOptions](./gettextoptions/) | يعيد خيارات النص. |

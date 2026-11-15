---
title: "FractionEquationNode فئة"
linktitle: "FractionEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "FractionEquationNode فئة. يغلف الكائن الذي يمثل fractionequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/fractionequationnode/
---

## FractionEquationNode class

هذه الفئة تحدد معادلة الكسر، وتتكون من بسط ومقام مفصولين بشريط كسر. يمكن أن يكون شريط الكسر أفقيًا أو مائلًا، حسب خصائص الكسر. تُستخدم معادلة الكسر أيضًا لتمثيل دالة التكديس، التي تضع عنصرًا فوق آخر دون شريط كسر.

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetFractionType](./getfractiontype/) | هذا يحدد نوع الكسر؛ الافتراضي هو 'Bar'. |
| [SetFractionType](./setfractiontype/) | هذا يحدد نوع الكسر؛ الافتراضي هو 'Bar'. |
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
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

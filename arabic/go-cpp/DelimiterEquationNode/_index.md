---
title: "فئة DelimiterEquationNode"
linktitle: "DelimiterEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة DelimiterEquationNode. تغلف الكائن الذي يمثل delimiterequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

هذه الفئة تحدد معادلة الفاصل، وتتكون من فواصل افتتاحية وإغلاقية (مثل الأقواس المستديرة، الأقواس المعقوفة، الأقواس المربعة، والشرطات العمودية)، ومكوّن موجود بداخلها. قد يحتوي الفاصل على أكثر من مكوّن، مع حرف فاصل مخصص بين كل مكوّن.

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetBeginChar](./getbeginchar/) | حرف بداية الفاصل. |
| [SetBeginChar](./setbeginchar/) | حرف بداية الفاصل. |
| [GetEndChar](./getendchar/) | حرف نهاية الفاصل. |
| [SetEndChar](./setendchar/) | حرف نهاية الفاصل. |
| [GetNaryGrow](./getnarygrow/) | يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة. |
| [SetNaryGrow](./setnarygrow/) | يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة. |
| [GetSeparatorChar](./getseparatorchar/) | حرف الفاصل. |
| [SetSeparatorChar](./setseparatorchar/) | حرف الفاصل. |
| [GetDelimiterShape](./getdelimitershape/) | يحدد شكل الفواصل في كائن الفاصل. |
| [SetDelimiterShape](./setdelimitershape/) | يحدد شكل الفواصل في كائن الفاصل. |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

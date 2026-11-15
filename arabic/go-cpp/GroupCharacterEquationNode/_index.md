---
title: "فئة GroupCharacterEquationNode"
linktitle: "GroupCharacterEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة GroupCharacterEquationNode. تغلف الكائن الذي يمثل groupcharacterequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/groupcharacterequationnode/
---

## GroupCharacterEquationNode class

هذه الفئة تحدد دالة تجميع-الحرف، وتتكون من حرف يُرسم فوق أو تحت النص، غالبًا بهدف تجميع العناصر بصريًا.

```go

type GroupCharacterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewGroupCharacterEquationNode](./newgroupcharacterequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetGroupChr](./getgroupchr/) | يحدد رمزًا (الافتراضي U+23DF). يُنصح بشدة باستخدام السمة ChrType لتعيين حرف التشكيل. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [SetGroupChr](./setgroupchr/) | يحدد رمزًا (الافتراضي U+23DF). يُنصح بشدة باستخدام السمة ChrType لتعيين حرف التشكيل. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [GetChrType](./getchrtype/) | حدد الأحرف المركبة حسب قيمة النوع. |
| [SetChrType](./setchrtype/) | حدد الأحرف المركبة حسب قيمة النوع. |
| [GetPosition](./getposition/) | هذه السمة تحدد موضع الحرف في الكائن |
| [SetPosition](./setposition/) | هذه السمة تحدد موضع الحرف في الكائن |
| [GetVertJc](./getvertjc/) | هذه السمة، بالاشتراك مع pos في groupChrPr، تحدد التخطيط العمودي لكائن groupChr. حيث يحدد pos موضع حرف التجميع، ويحدد vertJc محاذاة الكائن بالنسبة للخط الأساسي. |
| [SetVertJc](./setvertjc/) | هذه السمة، بالاشتراك مع pos في groupChrPr، تحدد التخطيط العمودي لكائن groupChr. حيث يحدد pos موضع حرف التجميع، ويحدد vertJc محاذاة الكائن بالنسبة للخط الأساسي. |
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
| [GroupCharacterEquationNode_CreateNode](./groupcharacterequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

---
title: "فئة AccentEquationNode"
linktitle: "AccentEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة AccentEquationNode. تغلف الكائن الذي يمثل accentequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/accentequationnode/
---

## AccentEquationNode class

هذه الفئة تحدد معادلة لهجة، تتكون من مكوّن أساسي وعلامة تشكيل مركبة.

```go

type AccentEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewAccentEquationNode](./newaccentequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetAccentCharacter](./getaccentcharacter/) | هذه الخاصية تحدد نوع علامة التشكيل المركبة المرفقة بقاعدة وظيفة التنوين. الحرف التنويني الافتراضي هو U+0302.يوصى بشدة استخدام الخاصية AccentType لتعيين حرف التنوين.استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [SetAccentCharacter](./setaccentcharacter/) | هذه الخاصية تحدد نوع علامة التشكيل المركبة المرفقة بقاعدة وظيفة التنوين. الحرف التنويني الافتراضي هو U+0302.يوصى بشدة استخدام الخاصية AccentType لتعيين حرف التنوين.استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [GetAccentCharacterType](./getaccentcharactertype/) | حدد الأحرف المركبة حسب قيمة النوع. |
| [SetAccentCharacterType](./setaccentcharactertype/) | حدد الأحرف المركبة حسب قيمة النوع. |
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
| [AccentEquationNode_CreateNode](./accentequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

---
title: "فئة NaryEquationNode"
linktitle: "NaryEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة NaryEquationNode. تغلف الكائن الذي يمثل naryequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/naryequationnode/
---

## NaryEquationNode class

هذه الفئة تحدد معادلة عامل n-ary، وتتكون من عامل n-ary، قاعدة (أو مُعامل)، وحدود علوية وسفلية اختيارية.

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [IsHideSubscript](./ishidesubscript/) | ما إذا كان سيتم عرض الحد الأدنى |
| [SetIsHideSubscript](./setishidesubscript/) | ما إذا كان سيتم عرض الحد الأدنى |
| [IsHideSuperscript](./ishidesuperscript/) | ما إذا كان سيتم عرض الحد الأقصى |
| [SetIsHideSuperscript](./setishidesuperscript/) | ما إذا كان سيتم عرض الحد الأقصى |
| [GetLimitLocation](./getlimitlocation/) | تحدد هذه السمة موقع الحدود في العوامل n-ary. يمكن أن تكون الحدود متمركزة إما فوق وتحت العامل n-ary، أو موضوعة مباشرةً إلى يمين العامل. |
| [SetLimitLocation](./setlimitlocation/) | تحدد هذه السمة موقع الحدود في العوامل n-ary. يمكن أن تكون الحدود متمركزة إما فوق وتحت العامل n-ary، أو موضوعة مباشرةً إلى يمين العامل. |
| [GetNaryOperator](./getnaryoperator/) | عامل n-ary. على سبيل المثال "∑". يُنصح بشدة باستخدام السمة NaryOperatorType لتعيين عامل n-ary. استخدم هذا الإعداد إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [SetNaryOperator](./setnaryoperator/) | عامل n-ary. على سبيل المثال "∑". يُنصح بشدة باستخدام السمة NaryOperatorType لتعيين عامل n-ary. استخدم هذا الإعداد إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [GetNaryOperatorType](./getnaryoperatortype/) | عامل n-ary. على سبيل المثال "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | عامل n-ary. على سبيل المثال "∑" |
| [GetNaryGrow](./getnarygrow/) | تحدد هذه السمة خاصية النمو للعوامل n-ary على مستوى المستند. عندما تكون معطلة، لا تنمو العوامل n-ary مثل التكاملات والمجاميع لتطابق حجم ارتفاع المعامل. عندما تكون مفعلة، ينمو العامل n-ary عموديًا ليتطابق مع ارتفاع معاملاته. |
| [SetNaryGrow](./setnarygrow/) | تحدد هذه السمة خاصية النمو للعوامل n-ary على مستوى المستند. عندما تكون معطلة، لا تنمو العوامل n-ary مثل التكاملات والمجاميع لتطابق حجم ارتفاع المعامل. عندما تكون مفعلة، ينمو العامل n-ary عموديًا ليتطابق مع ارتفاع معاملاته. |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

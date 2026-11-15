---
title: "فئة MatrixEquationNode"
linktitle: "MatrixEquationNode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة MatrixEquationNode. تغلف الكائن الذي يمثل matrixequationnode في Go."
type: docs
weight: 200
url: /ar/go-cpp/matrixequationnode/
---

## MatrixEquationNode class

هذه الفئة تحدد معادلة المصفوفة، وتتكون من عنصر واحد أو أكثر مُرتَّب في صف واحد أو أكثر وعمود واحد أو أكثر.

```go

type MatrixEquationNode struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewMatrixEquationNode](./newmatrixequationnode/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetBaseJc](./getbasejc/) | تحدد هذه الخاصية محاذاة المصفوفة. يمكن محاذاة النص خارج المصفوفة إلى الأسفل أو الأعلى أو الوسط لدالة المصفوفة. بشكل افتراضي، تفترض المصفوفة محاذاة مركزية. |
| [SetBaseJc](./setbasejc/) | تحدد هذه الخاصية محاذاة المصفوفة. يمكن محاذاة النص خارج المصفوفة إلى الأسفل أو الأعلى أو الوسط لدالة المصفوفة. بشكل افتراضي، تفترض المصفوفة محاذاة مركزية. |
| [IsHidePlaceholder](./ishideplaceholder/) | تحدد هذه الخاصية خاصية إخفاء العناصر النائبة على المصفوفة. عندما تكون هذه الخاصية مفعلة، لا تظهر العناصر النائبة في المصفوفة. بشكل افتراضي، تظهر العناصر النائبة بحيث تكون المواقع التي يمكن إدراج النص فيها مرئية. |
| [SetIsHidePlaceholder](./setishideplaceholder/) | تحدد هذه الخاصية خاصية إخفاء العناصر النائبة على المصفوفة. عندما تكون هذه الخاصية مفعلة، لا تظهر العناصر النائبة في المصفوفة. بشكل افتراضي، تظهر العناصر النائبة بحيث تكون المواقع التي يمكن إدراج النص فيها مرئية. |
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
| [MatrixEquationNode_CreateNode](./matrixequationnode_createnode/) | أنشئ عقدة من النوع المحدد. |

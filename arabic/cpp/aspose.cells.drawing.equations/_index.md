---
title: Aspose::Cells::Drawing::Equations namespace
linktitle: Aspose::Cells::Drawing::Equations
second_title: Aspose.Cells مرجع API لـ C++
description: 'كيفية استخدام مساحة الأسماء Aspose::Cells::Drawing::Equations في C++.'
type: docs
weight: 600
url: /ar/cpp/aspose.cells.drawing.equations/
---



## الفئات

| فئة | الوصف |
| --- | --- |
| [AccentEquationNode](./accentequationnode/) | هذه الفئة تحدد معادلة لهجة، تتكون من مكوّن أساسي ومكوّن صوتي مركب. |
| [ArrayEquationNode](./arrayequationnode/) | يحدد دالة Equation-Array، كائن يتكون من معادلة واحدة أو أكثر. |
| [BarEquationNode](./barequationnode/) | هذه الفئة تحدد معادلة الشريط، تتكون من حجة أساسية وشريط فوقي أو سفلي. |
| [BorderBoxEquationNode](./borderboxequationnode/) | هذه الفئة تحدد دالة [Border](../aspose.cells/border/) Box، تتكون من حد مرسوم حول معادلة. |
| [BoxEquationNode](./boxequationnode/) | هذه الفئة تحدد دالة الصندوق، التي تُستخدم لتجميع مكوّنات معادلة. |
| [DelimiterEquationNode](./delimiterequationnode/) | هذه الفئة تحدد معادلة الفاصل، تتكون من فواصل افتتاحية وإغلاقية (مثل الأقواس المستديرة، الأقواس المعقوفة، الأقواس المربعة، والشرطات الرأسية)، ومكوّن داخلها. قد يحتوي الفاصل على أكثر من مكوّن، مع حرف فاصل مخصص بين كل مكوّن. |
| [EquationComponentNode](./equationcomponentnode/) | هذه الفئة تحدد مكوّنات معادلة أو تعبير رياضي. تُدمج أنواع مختلفة من المكوّنات في معادلات مختلفة. على سبيل المثال، الكسر يتكون من جزأين، مكوّن البسط ومكوّن المقام. للمزيد من أنواع المكوّنات، يرجى الرجوع إلى 'EquationNodeType'. |
| [EquationNode](./equationnode/) | فئة مجردة لاشتقاق عقد معادلة أخرى. |
| [EquationNodeParagraph](./equationnodeparagraph/) | هذه الفئة تحدد فقرة رياضية تحتوي على عنصر واحد أو أكثر من MathEquationNode(OMath). |
| [FractionEquationNode](./fractionequationnode/) | هذه الفئة تحدد معادلة الكسر، التي تتكون من البسط والمقام مفصولين بشريط الكسر. يمكن أن يكون شريط الكسر أفقيًا أو مائلًا، حسب خصائص الكسر. تُستخدم معادلة الكسر أيضًا لتمثيل دالة التكديس، التي تضع عنصرًا فوق آخر دون شريط كسر. |
| [FunctionEquationNode](./functionequationnode/) | هذه الفئة تحدد معادلة تطبيق الدالة، التي تتكون من اسم الدالة وحجة تُطبق عليها. أنواع مكوّنات الاسم والحجة هي '[EquationNodeType.FunctionName](./equationnodetype/)' و'[EquationNodeType.Base](./equationnodetype/)' على التوالي. |
| [GroupCharacterEquationNode](./groupcharacterequationnode/) | هذه الفئة تحدد دالة تجميع الأحرف، التي تتكون من حرف يُرسم فوق أو تحت النص، غالبًا بهدف تجميع العناصر بصريًا. |
| [LimLowUppEquationNode](./limlowuppequationnode/) | هذه الفئة تحدد دالة الحد. |
| [MathematicalEquationNode](./mathematicalequationnode/) | هذه الفئة تحدد معادلة أو تعبير رياضي. جميع النصوص الرياضية للمعادلات أو التعابير الرياضية تُحتوى في هذه الفئة. |
| [MatrixEquationNode](./matrixequationnode/) | هذه الفئة تحدد معادلة المصفوفة، التي تتكون من عنصر واحد أو أكثر مُرتَّبة في صف واحد أو أكثر وعمود واحد أو أكثر. |
| [NaryEquationNode](./naryequationnode/) | هذه الفئة تحدد معادلة عامل n-ary، التي تتكون من عامل n-ary، قاعدة (أو مُعامل)، وحدود علوية وسفلية اختيارية. |
| [RadicalEquationNode](./radicalequationnode/) | هذه الفئة تحدد معادلة الجذر، التي تتكون من درجة اختيارية deg([EquationNodeType.Degree](./equationnodetype/)) وقاعدة. |
| [SubSupEquationNode](./subsupequationnode/) | هذه الفئة تحدد معادلة يمكن أن تكون اختيارياً فوقية أو تحتية. هناك أربع صيغ رئيسية لهذه المعادلة: فوقية، تحتية، فوقية وتحتية موضوعة إلى يسار القاعدة، وفوقية وتحتية موضوعة إلى يمين القاعدة. |
| [TextRunEquationNode](./textrunequationnode/) | هذه الفئة في عقدة المعادلة تُستخدم لتخزين المحتوى الفعلي (تسلسل من النص الرياضي) للمعادلة. عادةً يكون هناك كائن عقدة لكل حرف. |
| [UnknowEquationNode](./unknowequationnode/) | فئة عقدة المعادلة من نوع غير معروف. |
## Enums

| تعداد | الوصف |
| --- | --- |
| [EquationCharacterPositionType](./equationcharacterpositiontype/) | يحدد موضع كائن فرعي معين داخل العنصر الأصلي. |
| [EquationCombiningCharacterType](./equationcombiningcharactertype/) | نوع الأحرف المركبة. |
| [EquationDelimiterShapeType](./equationdelimitershapetype/) | هذا يحدد شكل الفواصل في كائن الفاصل. |
| [EquationFractionType](./equationfractiontype/) | هذا يحدد نمط عرض شريط الكسر. |
| [EquationHorizontalJustificationType](./equationhorizontaljustificationtype/) | هذا يحدد المحاذاة الأفقية الافتراضية للمعادلات في المستند. |
| [EquationLimitLocationType](./equationlimitlocationtype/) | يحدد موقع الحد على العامل. |
| [EquationMathematicalOperatorType](./equationmathematicaloperatortype/) | نوع عوامل الرياضيات. |
| [EquationNodeType](./equationnodetype/) | نوع عقدة المعادلة. ملاحظة: (1)[1-99] حاليًا هناك عقدة واحدة فقط في النطاق، وقيمة تعدادها هي 1. العقدة التي تحددها تُستخدم لتخزين النص الرياضي. (2)[100-199] تشير إلى أن العقدة مكوّن لبعض عقد الدوال الخاصة. (3)[200-] تشير إلى أن العقدة لها بعض الدوال الخاصة. |
| [EquationVerticalJustificationType](./equationverticaljustificationtype/) | هذا يحدد المحاذاة العمودية الافتراضية للمعادلات في المستند. |

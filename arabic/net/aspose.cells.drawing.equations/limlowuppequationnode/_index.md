---
title: "الفئة LimLowUppEquationNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Equations.LimLowUppEquationNode. تحدد هذه الفئة دالة الحد"
type: docs
url: /ar/net/aspose.cells.drawing.equations/limlowuppequationnode/
---
## LimLowUppEquationNode class

هذه الفئة تحدد دالة الحد.

```csharp
public class LimLowUppEquationNode : EquationNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | احصل على نوع المعادلة للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | يحدد العقدة الأب للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | يمثل نوع العقدة (موروث من [`EquationNode`](../equationnode/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/limlowuppequationnode/equals/)(object) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | إرجاع العقدة عند الفهرس المحدد بين أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | إدراج العقدة المحددة بعد العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | إدراج العقدة المحددة قبل العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | إدراج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | إزالة نفسها من الأصل. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | إزالة جميع العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | إزالة العقدة المحددة من أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | إزالة العقدة عند الفهرس المحدد من أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | تعيين نمط WordArt المسبق. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | تحويل هذه المعادلة إلى تعبير LaTeX. (موروث من [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | تحويل هذه المعادلة إلى تعبير MathML. (موروث من [`EquationNode`](../equationnode/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassLimLowUppEquationNodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء نسخة من الفئة LimLowUppEquationNode
                // نظرًا لعدم وجود مُنشئ عام بدون معلمات في الفئة،
                // سنستخدم نهجًا مختلفًا لعرض الوظيفة
                LimLowUppEquationNode limNode = null;
                LimLowUppEquationNode anotherNode = null;

                // عرض الوظيفة الأساسية - التحقق من مساواة الكائن
                bool areEqual = limNode?.Equals((object)anotherNode) ?? false;

                Console.WriteLine($"LimLowUppEquationNode demonstration");
                Console.WriteLine($"Nodes are equal: {areEqual}");

                // احفظ المصنف
                workbook.Save("LimLowUppEquationNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LimLowUppEquationNode: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



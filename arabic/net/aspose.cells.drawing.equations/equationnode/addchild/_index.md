---
title: "EquationNode.AddChild"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة EquationNode. إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| equationType | EquationNodeType | أنواع عقد المعادلة |

### قيمة الإرجاع

إذا كان النوع المحدد موجودًا، يتم إرجاع العقدة المقابلة، وإذا لم يكن النوع موجودًا، يتم إرجاع عقدة من نوع غير معروف.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة شكل معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على عقدة الرياضيات الجذرية
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة دالة وإضافة أبناء
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // إضافة اسم الدالة مع رفع
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // إضافة النص الأساسي لاسم الدالة
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // إضافة نص فوقي
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // إضافة معامل الدالة
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // احفظ المصنف
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية.

```csharp
public void AddChild(EquationNode node)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| العقدة | EquationNode | العقدة المحددة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل معادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // إنشاء عقدة نصية لتكون كأصل
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // إنشاء عقدة فرعية للإضافة باستخدام الطريقة الثابتة CreateNode
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // استدعاء طريقة AddChild مع معامل EquationNode
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // احفظ المصنف
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



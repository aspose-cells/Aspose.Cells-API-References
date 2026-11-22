---
title: "تعداد EquationCharacterPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Equations.EquationCharacterPositionType تعداد. يحدد موضع كائن فرعي معين داخل الكائن الأصل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

يحدد موضع كائن فرعي معين داخل الأصل الخاص به

```csharp
public enum EquationCharacterPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Top | `0` | في أعلى الكائن الأصل |
| Bottom | `1` | في أسفل الكائن الأصل |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCharacterPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // احصل على عقدة المعادلة وأضف شريطًا في الموضع العلوي
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            barNode.BarPosition = EquationCharacterPositionType.Top;
            
            // أضف النص الأساسي
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";
            
            // حفظ والتحقق
            string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
            workbook.Save(outputFile);
            
            // أعد التحميل وتحقق
            Workbook loadedWorkbook = new Workbook(outputFile);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
            Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



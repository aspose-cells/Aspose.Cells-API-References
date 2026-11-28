---
title: "Enum EquationLimitLocationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Bir operatör üzerindeki limit konumunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Bir operatör üzerindeki limit konumunu belirtir.

```csharp
public enum EquationLimitLocationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| UndOvr | `0` | Limitin operatörün üzerinde ya da altında ortalandığını belirtir. |
| SubSup | `1` | Limitin operatörün sağ tarafında olduğunu belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına bir denklem şekli ekleyin
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Denklem paragrafını ve ilk çocuğunu alın
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Bir Nary denklem düğümü oluşturun
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Limit konumunu SubSup (operatörün sağ tarafı) olarak ayarlayın
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Denkleme biraz içerik ekleyin
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // UndOvr'ye değiştirin (operatörün üzerinde/altında ortalanmış)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Çalışma kitabını kaydedin
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



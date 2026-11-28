---
title: "ShapeCollection.AddEquation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına bir denklem nesnesi ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Çalışma sayfasına bir denklem nesnesi ekler.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Üst satır indeksi. |
| üst | Int32 | Üst satırının dikey kayması, piksel biriminde. |
| leftColumn | Int32 | Sol sütun indeksi. |
| sol | Int32 | Sol sütunundan yatay kaydırma, piksel biriminde. |
| yükseklik | Int32 | Denklemin yüksekliği, piksel biriminde. |
| genişlik | Int32 | Denklemin genişliği, piksel biriminde. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fraction.FractionType = EquationFractionType.Skewed;

            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numText.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denText.Text = "B";

            workbook.Save("ShapeEquationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



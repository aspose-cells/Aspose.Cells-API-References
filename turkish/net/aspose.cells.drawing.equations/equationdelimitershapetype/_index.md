---
title: "Enum EquationDelimiterShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType enum. Bu, sınırlayıcı nesnesindeki sınırlayıcıların şeklini belirtir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Bu, sınırlayıcı nesnedeki sınırlayıcıların şeklini belirtir.

```csharp
public enum EquationDelimiterShapeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Centered | `0` | Bölücü, içeriğinin tüm yüksekliği etrafında ortalanmıştır. |
| Match | `1` | Bölücü, içeriklerinin yüksekliğine tam olarak uyması için ayarlanmıştır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Denklem şekli ekle
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Denklem düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Match şekil tipiyle bir sınırlayıcı düğümü oluştur
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Sınırlayıcının içine içerik ekle
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Çalışma kitabını kaydedin
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



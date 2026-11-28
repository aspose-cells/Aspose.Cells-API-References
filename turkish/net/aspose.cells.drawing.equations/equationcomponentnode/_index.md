---
title: "Sınıf EquationComponentNode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationComponentNode sınıfı. Bu sınıf bir denklem veya matematiksel ifadenin bileşenlerini belirtir. Farklı bileşen türleri farklı denklemlerde birleştirilir. Örneğin bir kesir iki parçadan oluşur: bir pay bileşeni ve bir payda bileşeni. Daha fazla bileşen türü için lütfen EquationNodeType'a bakın."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationcomponentnode/
---
## EquationComponentNode class

Bu sınıf, bir denklem veya matematiksel ifadenin bileşenlerini tanımlar. Farklı bileşen tipleri farklı denklemlerde birleştirilir. Örneğin, bir kesir iki parçadan oluşur: bir pay bileşeni ve bir payda bileşeni. Daha fazla bileşen türü için lütfen 'EquationNodeType' bölümüne bakın.

```csharp
public class EquationComponentNode : EquationNode
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Geçerli düğümün denklem türünü al (Miras alınan [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Karakterlerin uzunluğunu alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Geçerli düğümün üst düğümünü belirtir (Miras alınan [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Karakterlerin başlangıç indeksini alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Metin seçeneklerini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Düğümün türünü temsil eder (Miras alınan [`EquationNode`](../equationnode/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Belirtilen düğümü, geçerli düğümün alt düğüm listesinde sonuna ekler (Miras alınan [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Belirtilen tipte bir düğümü geçerli düğümün alt düğüm listesine sonuna ekle. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/equationcomponentnode/equals/)(object) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Geçerli düğümün çocukları arasında belirtilen indeksteki düğümü döndürür. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Belirtilen düğümü geçerli düğümün sonrasına ekler. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Belirtilen düğümü geçerli düğümün önüne ekler. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Belirtilen tipte bir düğümü geçerli düğümün alt düğüm listesinde belirtilen indeks konumuna ekler. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Kendisini üst düğümden kaldırır. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Geçerli düğümün tüm alt düğümlerini kaldırır. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Belirtilen düğümü geçerli düğümün çocuklarından kaldırır. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Belirtilen indeksteki düğümü geçerli düğümün çocuklarından kaldırır. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Önceden ayarlanmış WordArt stilini ayarlar. (Şuradan devralınmıştır [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Bu denklemi LaTeX ifadesine dönüştür. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Bu denklemi MathML ifadesine dönüştür. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationComponentNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Matematik düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Kesir düğümü oluştur
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Payı ekle
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "X";

            // Payda ekle
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "Y";

            // Kaydet ve doğrula
            workbook.Save("EquationComponentNodeDemo.xlsx");
            
            Console.WriteLine("Equation with component nodes created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



---
title: "Sınıf FunctionEquationNode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.FunctionEquationNode sınıfı. Bu sınıf, bir fonksiyon adı ve üzerine uygulanan bir argümandan oluşan FunctionApply denklemini tanımlar. Ad ve argüman bileşenlerinin türleri sırasıyla EquationNodeType.FunctionName ve EquationNodeType.Base'dir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/functionequationnode/
---
## FunctionEquationNode class

Bu sınıf, bir fonksiyon adı ve üzerine uygulanan bir argümandan oluşan Function-Apply denklemini belirtir. Ad ve argüman bileşenlerinin türleri sırasıyla 'EquationNodeType.FunctionName' ve 'EquationNodeType.Base' dir.

```csharp
public class FunctionEquationNode : EquationNode
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
| override [Equals](../../aspose.cells.drawing.equations/functionequationnode/equals/)(object) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
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
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassFunctionEquationNodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem ekle
            Worksheet worksheet = workbook.Worksheets[0];
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Denklemin kök düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Üst simgeli adla bir fonksiyon düğümü oluştur
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);

            // Üst simgeyle fonksiyon adı ekle
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);

            // Fonksiyon adı için temel metni ekle
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";

            // Üst simge metni ekle
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";

            // Fonksiyon argümanını ekle
            EquationNode baseArg = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argText = (TextRunEquationNode)baseArg.AddChild(EquationNodeType.Text);
            argText.Text = "x";

            // Çalışma kitabını kaydedin
            workbook.Save("FunctionEquationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



---
title: "Sınıf RadicalEquationNode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.RadicalEquationNode sınıfı. Bu sınıf, isteğe bağlı bir derece degEquationNodeType.Degree ve bir temel içeren radikal denklemi belirtir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/radicalequationnode/
---
## RadicalEquationNode class

Bu sınıf, isteğe bağlı bir derece deg(EquationNodeType.Degree) ve bir temel içeren radical denklemini belirtir.

```csharp
public class RadicalEquationNode : EquationNode
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Geçerli düğümün denklem türünü al (Miras alınan [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsDegHide](../../aspose.cells.drawing.equations/radicalequationnode/isdeghide/) { get; set; } | Radikallerin derecesini gizleyip gizlemeyeceği. |
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
| override [Equals](../../aspose.cells.drawing.equations/radicalequationnode/equals/)(object) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
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
    public class EquationsClassRadicalEquationNodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına denklem içeren bir metin kutusu ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklem düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bir radikal denklem düğümü ekleyin.
            RadicalEquationNode radicalNode = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
            radicalNode.IsDegHide = true;

            // Dereceyi (gizli) ve temel bileşenleri ekleyin.
            EquationNode degreeNode = radicalNode.AddChild(EquationNodeType.Degree);
            TextRunEquationNode degreeText = (TextRunEquationNode)degreeNode.AddChild(EquationNodeType.Text);
            degreeText.Text = "3";

            EquationNode baseNode = radicalNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x + 1";

            // Çalışma kitabını kaydedin
            workbook.Save("RadicalEquationDemo.xlsx");

            // Kaydedilmiş çalışma kitabını doğrulamak için yükle
            Workbook loadedWorkbook = new Workbook("RadicalEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            RadicalEquationNode loadedRadicalNode = (RadicalEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("Radical equation created successfully:");
            Console.WriteLine($"- IsDegHide: {loadedRadicalNode.IsDegHide}");
            Console.WriteLine($"- Base text: {((TextRunEquationNode)loadedRadicalNode.GetChild(1).GetChild(0)).Text}");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



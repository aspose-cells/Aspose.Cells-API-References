---
title: "Sınıf TextRunEquationNode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.TextRunEquationNode sınıfı. Bu sınıf, denklem düğümünde denklemin gerçek içeriği olan matematiksel metin dizisini depolamak için kullanılır. Genellikle karakter başına bir düğüm nesnesi bulunur"
type: docs
url: /tr/net/aspose.cells.drawing.equations/textrunequationnode/
---
## TextRunEquationNode class

Bu sınıf, denklem düğümünde denklemin gerçek içeriğini (bir matematiksel metin dizisi) depolamak için kullanılır. Genellikle karakter başına bir düğüm nesnesi.

```csharp
public class TextRunEquationNode : EquationNode
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Geçerli düğümün denklem türünü al (Miras alınan [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Karakterlerin uzunluğunu alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Geçerli düğümün üst düğümünü belirtir (Miras alınan [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Karakterlerin başlangıç indeksini alır (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Text](../../aspose.cells.drawing.equations/textrunequationnode/text/) { get; set; } | Metin düğümünün içeriğini ayarla (Genellikle karakter başına bir düğüm nesnesi). |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Metin seçeneklerini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Düğümün türünü temsil eder (Miras alınan [`EquationNode`](../equationnode/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Belirtilen düğümü, geçerli düğümün alt düğüm listesinde sonuna ekler (Miras alınan [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Belirtilen tipte bir düğümü geçerli düğümün alt düğüm listesine sonuna ekle. (Şuradan devralınmıştır [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/textrunequationnode/equals/)(object) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
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
    public class EquationsClassTextRunEquationNodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına denklem içeren bir metin kutusu ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Denklem paragrafından matematik düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bir kenarlık kutusu düğümü oluştur
            BorderBoxEquationNode borderBoxNode = (BorderBoxEquationNode)mathNode.AddChild(EquationNodeType.BorderBox);

            // Temel düğümü kenarlık kutusuna ekle
            EquationNode baseNode = borderBoxNode.AddChild(EquationNodeType.Base);

            // Metin çalıştırma düğümünü temel düğüme ekle ve metnini ayarla
            TextRunEquationNode textRunNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textRunNode.Text = "x + y = z";

            // Çalışma kitabını kaydedin
            workbook.Save("TextRunEquationNodeDemo.xlsx");

            Console.WriteLine("Equation with TextRun node created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



---
title: "Class EquationNodeParagraph"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Equations.EquationNodeParagraph sınıfı. Bu sınıf, bir veya daha fazla MathEquationNodeOMath öğesi içeren bir matematik paragrafını belirtir."
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnodeparagraph/
---
## EquationNodeParagraph class

Bu sınıf, bir veya daha fazla MathEquationNode(OMath) öğesi içeren matematiksel bir paragrafı tanımlar.

```csharp
public class EquationNodeParagraph : EquationNode
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Geçerli düğümün denklem türünü al (Miras alınan [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Bu nesnenin yazı tipini döndürür (Miras alınan [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Justification](../../aspose.cells.drawing.equations/equationnodeparagraph/justification/) { get; set; } | Bu, matematik paragrafının hizalamasını belirtir (aynı paragrafta yan yana bulunan bir dizi denklem). Bir matematik paragrafı Sol Hizalı, Sağ Hizalı, Ortalanmış veya Grup Olarak Ortalanmış olabilir. Varsayılan olarak, matematik paragrafı Grup Olarak Ortalanmıştır. Bu, denklemlerin birbirlerine göre hizalanabileceği, ancak tüm denklem grubunun bütün olarak ortalandığı anlamına gelir. |
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
| override [Equals](../../aspose.cells.drawing.equations/equationnodeparagraph/equals/)(object) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle |
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationNodeParagraphDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Denklem paragrafını tutacak bir şekil oluşturun
                var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

                // Şekilden denklem paragrafını alın
                var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

                if (equationParagraph != null)
                {
                    // Varsayılan hizalamayı gösterin
                    Console.WriteLine($"Default Justification: {equationParagraph.Justification}");

                    // Hizalamayı Sol olarak değiştirin
                    equationParagraph.Justification = EquationHorizontalJustificationType.Left;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // Hizalamayı Ortala olarak değiştir
                    equationParagraph.Justification = EquationHorizontalJustificationType.Center;
                    Console.WriteLine($"Justification changed to: {equationParagraph.Justification}");

                    // Çalışma kitabını kaydedin
                    workbook.Save("EquationNodeParagraphDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("Failed to get EquationNodeParagraph from shape.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationNodeParagraph: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)



---
title: "EquationNode.GetChild"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Mevcut düğümün alt düğümleri arasında belirtilen indeksteki düğümü döndürür"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Geçerli düğümün alt düğümleri arasında belirtilen indeksteki düğümü döndürür.

```csharp
public EquationNode GetChild(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Düğümün indeksi |

### Dönüş Değeri

Belirtilen düğüm mevcutsa ilgili düğümü döndürür, aksi takdirde null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodGetChildWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem şekli ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Denklemin paragrafını ve ilk alt düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Bir ayırıcı düğümünü alt düğüm olarak ekle
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Ayırıcı içinde bir kesir düğümü ekle
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Pay ve paydayı ekle
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Çalışma kitabını kaydedin
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Doğrulamak için kaydedilmiş dosyayı yükle
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // GetChild metodunu göster
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Delimiter BeginChar: " + loadedDelimiter.BeginChar);
            Console.WriteLine("Delimiter EndChar: " + loadedDelimiter.EndChar);
            
            EquationNode loadedBaseNode = loadedDelimiter.GetChild(0);
            FractionEquationNode loadedFraction = (FractionEquationNode)loadedBaseNode.GetChild(0);
            
            Console.WriteLine("Fraction node type: " + loadedFraction.EquationType);
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



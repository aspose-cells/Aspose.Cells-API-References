---
title: "TextBox.GetEquationParagraph"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBox yöntemi. TextBox nesnesinin TextBody özelliğinden belirtilen matematik paragrafını alın. Not 1: Dizin sınırların dışındaysa veya bulunamazsa NULL döndürür. 2: Belirtilen dizin konumu bir matematik paragrafı değilse de NULL döndürür."
type: docs
url: /tr/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

TextBox nesnesinin TextBody özelliğinden belirtilen matematik paragrafını alır. Not: (1) Dizin sınırların dışındaysa veya bulunamazsa NULL döndürür. (2) Ayrıca belirtilen dizin konumu bir matematik paragrafı değilse NULL döndürür.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Matematik paragrafının konum indeksi, 0'dan başlayarak. |

### Dönüş Değeri

Belirtilen indeksle matematik paragrafını döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class TextBoxMethodGetEquationParagraphWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Metin kutusuna bazı denklem içerikleri ekleyin
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // GetEquationParagraph metodunu indeks parametresi (Int32) ile çağırın
                EquationNode equationNode = textBox.GetEquationParagraph(0);

                if (equationNode != null)
                {
                    Console.WriteLine("Equation paragraph retrieved successfully.");
                    Console.WriteLine($"Equation type: {equationNode.EquationType}");
                    Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
                }
                else
                {
                    Console.WriteLine("No equation paragraph found at the specified index.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

TextBox nesnesinin TextBody özelliğinden ilk matematik paragrafını alır.

```csharp
public EquationNode GetEquationParagraph()
```

### Dönüş Değeri

Eğer bir matematik paragrafı varsa, ilkini döndürür, aksi takdirde null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextBoxMethodGetEquationParagraphDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "$$\\sqrt{x^2+y^2}$$";
            
            EquationNode equationNode = textBox.GetEquationParagraph();
            
            if (equationNode != null)
            {
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
            }
            else
            {
                Console.WriteLine("No equation paragraph found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



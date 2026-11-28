---
title: "EquationNode.AddChild"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Belirtilen türde bir düğümü, mevcut düğümün alt düğüm listesine sonuna ekleyin"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Belirtilen tipte bir düğümü geçerli düğümün alt düğüm listesinin sonuna ekle.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | EquationNodeType | Denklem Düğümlerinin Türleri |

### Dönüş Değeri

Belirtilen tür mevcutsa, karşılık gelen düğüm döndürülür; tür mevcut değilse, bilinmeyen türde bir düğüm döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem şekli ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Kök matematik düğümünü alın
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bir fonksiyon düğümü oluşturun ve alt düğümler ekleyin
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
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Çalışma kitabını kaydedin
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Belirtilen düğümü geçerli düğümün alt düğüm listesinde sonuna ekler.

```csharp
public void AddChild(EquationNode node)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| düğüm | EquationNode | Belirtilen düğüm |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir denklem şekli oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Üst düğüm olarak hizmet edecek bir metin düğümü oluştur
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Statik CreateNode yöntemiyle eklemek için bir alt düğüm oluştur
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // EquationNode parametresiyle AddChild yöntemini çağır
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Çalışma kitabını kaydedin
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



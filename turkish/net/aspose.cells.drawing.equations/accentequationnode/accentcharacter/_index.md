---
title: "AccentEquationNode.AccentCharacter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AccentEquationNode özelliği. Bu öznitelik, aksan işlevinin temeline eklenen birleştirici diakritik işaretin türünü belirtir. Varsayılan aksan karakteri U0302'dir. Aksan karakterini ayarlamak için AccentType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın."
type: docs
url: /tr/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Bu öznitelik, aksan işlevinin temeline eklenen birleştirici diakritik işaretin tipini belirtir. Varsayılan aksan karakteri U+0302'dir. Aksan karakterini ayarlamak için AccentType özniteliğini kullanmanız şiddetle önerilir. Bilinen bir tipte ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın.

```csharp
public string AccentCharacter { get; set; }
```

### Açıklamalar

Bu özelliğin yalnızca bir karakter kabul ettiğini ve birden fazla karakter gönderildiğinde sadece ilk karakterin kabul edildiğini belirtmek gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem şekli ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklem düğümünü alın ve bir aksan düğümü ekleyin
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Aksan karakterini ayarlayın (bu durumda şapka işareti)
            accentNode.AccentCharacter = "\u0302";

            // Aksan için temel metni ekleyin
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Çalışma kitabını kaydedin
            workbook.Save("AccentEquationDemo.xlsx");

            // Kaydedilen dosyayı geri yükleyerek doğrulayın
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Özelliği göstermek için aksan karakterini çıktıya verin
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Ayrıca Bakınız

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



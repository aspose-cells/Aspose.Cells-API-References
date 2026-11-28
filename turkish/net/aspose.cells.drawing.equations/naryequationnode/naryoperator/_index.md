---
title: "NaryEquationNode.NaryOperator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NaryEquationNode özelliği. bir nary operatör. örn. NaryOperatorType özniteliğini kullanarak nary operatör ayarlamanız şiddetle tavsiye edilir. Bilinen bir tipte ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın."
type: docs
url: /tr/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

n-ary bir operatör. örn. "∑". n-ary operatörü ayarlamak için NaryOperatorType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir türde ihtiyacınız olan karakteri bulamazsanız bu özellik ayarını kullanın.

```csharp
public string NaryOperator { get; set; }
```

### Açıklamalar

Bu özelliğin yalnızca bir karakter kabul ettiğini ve birden fazla karakter gönderildiğinde sadece ilk karakterin kabul edildiğini belirtmek gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir denklem şekli ekle
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Denklem düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Bir nary operatör düğümü oluştur
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // nary operatör özelliklerini ayarla
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Alt simge ekleyin (isteğe bağlı)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Üst simge ekleyin (isteğe bağlı)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Temel ifadeyi ekle
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Çalışma kitabını kaydedin
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



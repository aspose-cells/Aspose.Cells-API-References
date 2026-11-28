---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GroupCharacterEquationNode özelliği. Bu öznitelik, groupChrPr'nin pos özelliğiyle birleştirildiğinde groupChr nesnesinin dikey düzenini belirtir. pos, gruplayıcı karakterin konumunu belirtirken, vertJc nesnenin temel çizgiye göre hizalamasını belirler."
type: docs
url: /tr/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Bu öznitelik, groupChrPr'nin pos değeriyle birleştirildiğinde groupChr nesnesinin dikey düzenini belirtir. pos, gruplama karakterinin konumunu belirtirken, vertJc nesnenin temel çizgiye göre hizalamasını belirtir.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Denklemi içerecek bir metin kutusu şekli oluştur
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Bir GroupCharacterEquationNode örneği oluştur
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Denklem düğümü için başlangıç özelliklerini ayarla
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // VertJc özelliğini göster (okuma ve yazma)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // VertJc değerini değiştir
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Çalışma kitabını kaydedin
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



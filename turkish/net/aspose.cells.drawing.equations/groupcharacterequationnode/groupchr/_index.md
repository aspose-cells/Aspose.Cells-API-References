---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GroupCharacterEquationNode özelliği. Bir symboldefault U23DF belirtir. Aksan karakteri ayarlamak için ChrType özniteliğini kullanmanız şiddetle tavsiye edilir. Bilinen bir tipte ihtiyacınız olan karakteri bulamıyorsanız bu özellik ayarını kullanın."
type: docs
url: /tr/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Bir sembol (varsayılan U+23DF) belirtir. Aksan karakterini ayarlamak için ChrType özniteliğini kullanmanız şiddetle tavsiye edilir. Gerekli karakteri bilinen bir türde bulamıyorsanız bu özellik ayarını kullanın.

```csharp
public string GroupChr { get; set; }
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
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir denklem ekle
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Denklemin kök düğümünü al
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Sağa çift ok ile bir grup karakter düğümü oluştur
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Temel metni grup karakterine ekle
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // GroupChr özelliğinin kullanımını göster
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Çalışma kitabını kaydedin
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)



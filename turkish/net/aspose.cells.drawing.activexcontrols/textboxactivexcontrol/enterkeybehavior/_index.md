---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. ENTER tuşunun davranışını belirtir. True, ENTER'a basıldığında yeni bir satır oluşturulacağını belirtir. False, ENTER'a basıldığında odaklamanın sekme sırasındaki bir sonraki nesneye taşınacağını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

ENTER tuşunun davranışını belirtir. True, ENTER tuşuna basmanın yeni bir satır oluşturacağını belirtir. False, ENTER tuşuna basmanın odak noktasını sekme sırasındaki bir sonraki nesneye taşıyacağını belirtir.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterKeyBehaviorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir TextBox ActiveX Control ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // EnterKeyBehavior özelliğini göster
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // EnterKeyBehavior'ı değiştir
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



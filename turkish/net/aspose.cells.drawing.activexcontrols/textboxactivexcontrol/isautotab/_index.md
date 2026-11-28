---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki kontrole geçip geçmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Kullanıcı maksimum karakter sayısına ulaştığında odak noktasının otomatik olarak bir sonraki kontrole geçip geçmeyeceğini gösterir.

```csharp
public bool IsAutoTab { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir TextBox ActiveX kontrolü ekle ve kontrolünü al
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // IsAutoTab özelliğini göster
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // IsAutoTab false ise true olarak ayarla
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



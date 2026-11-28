---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ToggleButtonActiveXControl özelliği. Belirtilen kontrolün Null değerlerini nasıl göstereceğini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Belirtilen kontrolün Null değerlerini nasıl görüntüleyeceğini gösterir.

```csharp
public bool IsTripleState { get; set; }
```

### Açıklamalar

| **Ayar** | **Description** |
| --- | --- |
| Doğru | Kontrol, Evet, Hayır ve Null değerleri için durumlar arasında dönecektir. Kontrol, Value özelliği Null olarak ayarlandığında karartılmış (gri) görünür. |
| Yanlış | (Varsayılan) Kontrol, Evet ve Hayır değerleri için durumlar arasında dönecektir. Null değerler, Hayır değerleri gibi görüntülenir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ToggleButton ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // IsTripleState özelliğini true olarak ayarla
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // IsTripleState özelliğini false olarak değiştir
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Çalışma kitabını kaydedin
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



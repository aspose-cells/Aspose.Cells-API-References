---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. Belirtilen kontrolün Null değerleri nasıl görüntüleyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir CheckBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri yapılandırın
            checkBox.Caption = "Triple State Demo";
            
            // IsTripleState özelliğini gösterin
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



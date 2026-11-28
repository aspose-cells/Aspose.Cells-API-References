---
title: "ActiveXControlBase.ForeOleColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Ön planın ole rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Ön planın ole rengini alır ve ayarlar.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Açıklamalar

Görüntü kontrolü için geçerli değildir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir CheckBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri ayarlayın
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // ForeOleColor özelliğini gösterin
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // Çalışma kitabını kaydedin
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



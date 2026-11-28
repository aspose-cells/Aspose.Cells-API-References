---
title: "ActiveXControl.IsAutoSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControl özelliği. Kontrolün tüm içeriğini göstermek için otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

Kontrolün tüm içeriğini göstermek için otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını belirtir.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AddActiveXControl parametreleri tam imza ile düzeltildi
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 0, 0, 100, 50);
            ActiveXControl control = shape.ActiveXControl;

            Console.WriteLine("Initial IsAutoSize: " + control.IsAutoSize);
            control.IsAutoSize = true;
            Console.WriteLine("Set IsAutoSize: " + control.IsAutoSize);

            string outputPath = "AutoSizeControlDemo.xlsm";
            workbook.Save(outputPath, SaveFormat.Xlsm);

            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ActiveXControl loadedControl = loadedShape.ActiveXControl;
            Console.WriteLine("Loaded IsAutoSize: " + loadedControl.IsAutoSize);
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



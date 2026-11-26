---
title: "ActiveXControl.IsAutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Указывает, будет ли элемент управления автоматически изменять размер, чтобы отобразить всё его содержимое"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### Примеры

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

            // Исправлены параметры AddActiveXControl с полной сигнатурой
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

### См. также

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



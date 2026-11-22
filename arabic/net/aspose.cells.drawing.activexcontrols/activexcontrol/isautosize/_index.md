---
title: "ActiveXControl.IsAutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تشير إلى ما إذا كان التحكم سيعيد حجمه تلقائيًا لعرض جميع محتوياته"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### أمثلة

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

            // تم تصحيح معلمات AddActiveXControl مع التوقيع الكامل
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

### انظر أيضًا

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



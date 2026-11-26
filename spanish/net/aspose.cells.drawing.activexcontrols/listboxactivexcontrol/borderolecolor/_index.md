---
title: "ListBoxActiveXControl.BorderOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Obtiene y establece el color OLE del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderolecolor/
---
## ListBoxActiveXControl.BorderOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public int BorderOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 0, 0, 200, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            listBox.BorderOleColor = -2147483642;
            
            workbook.Save("ListBoxBorderOleColorDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



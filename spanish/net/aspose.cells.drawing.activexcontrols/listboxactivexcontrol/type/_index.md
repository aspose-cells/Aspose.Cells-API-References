---
title: "ListBoxActiveXControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/type/
---
## ListBoxActiveXControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un control ListBox ActiveX con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            // Demostrar la propiedad Type
            Console.WriteLine("Control Type: " + listBox.Type);
            
            // Establecer algunas propiedades
            listBox.ScrollBars = ControlScrollBarType.BarsBoth;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Single;
            
            // Verifique la propiedad Type
            if (listBox.Type == ControlType.ListBox)
            {
                Console.WriteLine("This is a ListBox control as expected");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



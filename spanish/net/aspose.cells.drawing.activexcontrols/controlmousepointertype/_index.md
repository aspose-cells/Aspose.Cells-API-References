---
title: "Enumeración ControlMousePointerType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType. Representa el tipo de ícono que se muestra como puntero del mouse para el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Representa el tipo de ícono mostrado como puntero del ratón para el control.

```csharp
public enum ControlMousePointerType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Puntero estándar. |
| Arrow | `1` | Flecha. |
| Cross | `2` | Puntero de mira cruzada. |
| IBeam | `3` | Cursor en forma de I. |
| SizeNESW | `6` | Doble flecha apuntando al noreste y suroeste. |
| SizeNS | `7` | Doble flecha apuntando al norte y al sur. |
| SizeNWSE | `8` | Doble flecha apuntando al noroeste y sureste. |
| SizeWE | `9` | Doble flecha apuntando al oeste y al este. |
| UpArrow | `10` | Flecha hacia arriba. |
| HourGlass | `11` | Reloj de arena. |
| NoDrop | `12` | Símbolo "No" (círculo con una línea diagonal) sobre el objeto que se está arrastrando. |
| AppStarting | `13` | Flecha con un reloj de arena. |
| Help | `14` | Flecha con un signo de interrogación. |
| SizeAll | `15` | Cursor "Tamaño todo" (flechas apuntando al norte, sur, este y oeste). |
| Custom | `99` | Utiliza el ícono especificado por la propiedad MouseIcon. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Convierta el ActiveXControl a ActiveXControlBase para acceder a sus propiedades
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Establezca el tipo de puntero del ratón para el control
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Establezca otras propiedades para la demostración
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Guarda el libro de trabajo
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Mostrar el resultado
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



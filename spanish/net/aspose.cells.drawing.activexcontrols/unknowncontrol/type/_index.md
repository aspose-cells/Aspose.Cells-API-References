---
title: "UnknownControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnknownControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Cargar libro de trabajo existente que contiene un control desconocido
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Buscar y procesar instancias de UnknownControl
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // Demostrar la lectura de la propiedad Type
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // Ejemplo de uso basado en el tipo de control
                    if (control.Type == ControlType.ListBox)
                    {
                        Console.WriteLine("Processing legacy ListBox control");
                    }
                    else if (control.Type == ControlType.Unknown)
                    {
                        Console.WriteLine("Handling completely unknown control type");
                    }
                }
            }

            // Guardar libro de trabajo procesado
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



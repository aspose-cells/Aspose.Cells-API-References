---
title: "ActiveXControlBase.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene el objeto Workbook"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Obtiene el objeto `Workbook`.

```csharp
public Workbook Workbook { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un control ActiveX a la hoja de cálculo
                Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

                // Establecer algunas propiedades para que el ejemplo tenga sentido
                checkBox.Caption = "Sample CheckBox";
                checkBox.IsAutoSize = true;

                // Demostrar la propiedad Workbook (solo lectura)
                Workbook controlWorkbook = checkBox.Workbook;
                Console.WriteLine("ActiveX Control Workbook reference obtained successfully.");
                Console.WriteLine("Workbook has " + controlWorkbook.Worksheets.Count + " worksheets.");

                // Verificar que la referencia del libro de trabajo sea la misma que nuestro libro de trabajo original
                if (controlWorkbook == workbook)
                {
                    Console.WriteLine("The ActiveX control's Workbook property correctly references the parent workbook.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ActiveXControlWorkbookDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



---
title: "ComboBoxActiveXControl.MatchEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/
---
## ComboBoxActiveXControl.MatchEntry property

Indica cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 20);
            
            // Obtener el control ComboBox ActiveX
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurar propiedades básicas
            comboBox.Font.Name = "Arial";
            comboBox.Font.Size = 10;
            comboBox.ListRows = 8;

            // Demostrar la propiedad MatchEntry
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
            Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);

            // Cambiar MatchEntry a otro modo
            comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
            Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



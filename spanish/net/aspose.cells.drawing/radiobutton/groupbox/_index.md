---
title: "RadioButton.GroupBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButton. Obtiene el GroupBox que contiene este RadioButton"
type: docs
url: /es/net/aspose.cells.drawing/radiobutton/groupbox/
---
## RadioButton.GroupBox property

Obtiene el GroupBox que contiene este RadioButton.

```csharp
public GroupBox GroupBox { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonPropertyGroupBoxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un GroupBox para contener botones de opción
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
            groupBox.Name = "OptionsGroup";
            groupBox.Shadow = true;

            // Agregar botones de opción a la hoja de cálculo (aún no en el GroupBox)
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);

            // Mostrar los valores iniciales de la propiedad GroupBox (debería ser nulo)
            Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
            Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));

            // Agregar botones de opción al GroupBox estableciendo la colocación
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;

            // Mover los botones de opción dentro del GroupBox
            radioButton1.Top = groupBox.Top + 20;
            radioButton1.Left = groupBox.Left + 20;
            radioButton2.Top = groupBox.Top + 50;
            radioButton2.Left = groupBox.Left + 20;

            // Mostrar los valores de la propiedad GroupBox después de agrupar
            Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
            Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);

            // Demostrar el comportamiento del grupo
            radioButton1.IsChecked = true;
            Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
            Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);

            // Guardar el resultado
            workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



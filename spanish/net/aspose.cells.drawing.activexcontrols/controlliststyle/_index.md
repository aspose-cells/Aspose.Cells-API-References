---
title: "Enum ControlListStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlListStyle enum. Representa la apariencia visual de la lista en un ListBox o ComboBox"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlliststyle/
---
## ControlListStyle enumeration

Representa la apariencia visual de la lista en un ListBox o ComboBox.

```csharp
public enum ControlListStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Plain | `0` | Muestra una lista en la que el fondo de un elemento se resalta cuando está seleccionado. |
| Option | `1` | Muestra una lista en la que un botón de opción o una casilla de verificación junto a cada entrada muestra el estado de selección de ese elemento. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlListStyleDemo
    {
        public static void ControlListStyleExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain

            // Agregar elementos al ComboBox
            comboBox.Value = "Item 1";
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;

            // Agregar un control ActiveX ListBox a la hoja de cálculo
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Establecer propiedades para el ListBox
            listBox.ColumnCount = 1;
            listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option

            // Agregar elementos al ListBox
            listBox.Value = "Item 1";
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;

            // Guarda el libro de trabajo
            workbook.Save("ControlListStyleExample.xlsx");
            workbook.Save("ControlListStyleExample.pdf");

            // Genere la salida de los resultados
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



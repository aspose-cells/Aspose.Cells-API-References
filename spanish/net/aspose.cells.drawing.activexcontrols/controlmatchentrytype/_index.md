---
title: "Enumeración ControlMatchEntryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType. Representa cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Representa cómo un ListBox o ComboBox busca en su lista mientras el usuario escribe.

```csharp
public enum ControlMatchEntryType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FirstLetter | `0` | El control busca la siguiente entrada que comienza con el carácter introducido. Escribir repetidamente la misma letra recorre todas las entradas que empiezan con esa letra. |
| Complete | `1` | A medida que se escribe cada carácter, el control busca una entrada que coincida con todos los caracteres ingresados. |
| None | `2` | La lista no se buscará cuando se escriban caracteres. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Agregar elementos al ComboBox
            comboBox.Value = "Apple;Banana;Cherry";

            // Agregar un control ActiveX ListBox a la hoja de cálculo
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Establecer propiedades para el ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Agregar elementos al ListBox
            listBox.Value = "Apple;Banana;Cherry";

            // Guarda el libro de trabajo
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Genere la salida de los resultados
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



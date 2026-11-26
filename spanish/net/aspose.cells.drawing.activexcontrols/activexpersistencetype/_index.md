---
title: "Enumeración ActiveXPersistenceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType. Representa el método de persistencia para guardar un control ActiveX."
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

Representa el método de persistencia para guardar un control ActiveX.

```csharp
public enum ActiveXPersistenceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| PropertyBag | `0` | Los datos se almacenan como datos XML. |
| Storage | `1` | Los datos se almacenan como datos binarios de almacenamiento. |
| Stream | `2` | Los datos se almacenan como datos binarios de flujo. |
| StreamInit | `3` | Los datos se almacenan como datos binarios de streaminit. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassActiveXPersistenceTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            // Agregue diferentes controles ActiveX para demostrar varios tipos de persistencia.
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);

            // Guarde el libro de trabajo con todos los controles ActiveX.
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // Agregue un control ActiveX.
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                row,
                15,
                column,
                15,
                200,
                50
            );

            // Configure el control según el tipo.
            switch (controlType)
            {
                case ControlType.CommandButton:
                    var button = (CommandButtonActiveXControl)shape.ActiveXControl;
                    button.IsVisible = true;
                    
                    button.Caption = $"{persistenceType} Button";
                    break;

                case ControlType.TextBox:
                    var textBox = (TextBoxActiveXControl)shape.ActiveXControl;
                    textBox.IsVisible = true;
                    textBox.Text = $"{persistenceType} TextBox";
                    break;

                case ControlType.CheckBox:
                    var checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                    checkBox.IsVisible = true;
                    checkBox.Caption = $"{persistenceType} CheckBox";
                    checkBox.Value = CheckValueType.Checked;
                    break;

                case ControlType.ComboBox:
                    var comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
                    comboBox.IsVisible = true;
                    comboBox.ListFillRange = $"A3:A7";
                    break;
            }

            // El tipo de persistencia es manejado internamente por Aspose.Cells al guardar.
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



---
title: Enum ActiveXPersistenceType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType enum. Represents the persistence method to persist an ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

Represents the persistence method to persist an ActiveX control.

```csharp
public enum ActiveXPersistenceType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| PropertyBag | `0` | The data is stored as xml data. |
| Storage | `1` | The data is stored as a storage binary data. |
| Stream | `2` | The data is stored as a stream binary data. |
| StreamInit | `3` | The data is stored as a streaminit binary data. |

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add different ActiveX controls to demonstrate various persistence types
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 0);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 2, 0);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 4, 0);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 6, 0);

            // Save the workbook with all ActiveX controls
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType, 
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // Add an ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                column,
                row,
                1500,
                1500,
                2000,
                500
            );

            // Configure control based on type
            switch (controlType)
            {
                case ControlType.CommandButton:
                    var button = (CommandButtonActiveXControl)shape.ActiveXControl;
                    button.Caption = $"{persistenceType} Button";
                    break;
                    
                case ControlType.TextBox:
                    var textBox = (TextBoxActiveXControl)shape.ActiveXControl;
                    textBox.Text = $"{persistenceType} TextBox";
                    break;
                    
                case ControlType.CheckBox:
                    var checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                    checkBox.Caption = $"{persistenceType} CheckBox";
                    checkBox.Value = CheckValueType.Checked;
                    break;
                    
                case ControlType.ComboBox:
                    var comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
                    comboBox.ListFillRange = $"A{row+1}:A{row+5}";
                    break;
            }

            // The persistence type is handled internally by Aspose.Cells when saving
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



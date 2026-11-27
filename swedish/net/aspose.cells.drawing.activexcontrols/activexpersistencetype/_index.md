---
title: "Enum ActiveXPersistenceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType-enum. Representerar persistensmetoden för att spara en ActiveX-kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

Representerar beständighetsmetoden för att spara en ActiveX-kontroll.

```csharp
public enum ActiveXPersistenceType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| PropertyBag | `0` | Data lagras som XML-data. |
| Storage | `1` | Data lagras som lagringsbinär data. |
| Stream | `2` | Data lagras som ström-binär data. |
| StreamInit | `3` | Data lagras som streaminit-binär data. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            // Lägg till olika ActiveX-kontroller för att demonstrera olika persistens-typer
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);

            // Spara arbetsboken med alla ActiveX-kontroller
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // Lägg till en ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                row,
                15,
                column,
                15,
                200,
                50
            );

            // Konfigurera kontroll baserat på typ
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

            // Persistenstypen hanteras internt av Aspose.Cells vid sparande
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



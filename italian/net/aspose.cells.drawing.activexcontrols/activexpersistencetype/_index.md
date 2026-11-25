---
title: "Enum ActiveXPersistenceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType enum. Rappresenta il metodo di persistenza per conservare un controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

Rappresenta il metodo di persistenza per conservare un controllo ActiveX.

```csharp
public enum ActiveXPersistenceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| PropertyBag | `0` | I dati sono memorizzati come dati XML. |
| Storage | `1` | I dati sono memorizzati come dati binari di archiviazione. |
| Stream | `2` | I dati sono memorizzati come dati binari di flusso. |
| StreamInit | `3` | I dati sono memorizzati come dati binari di streaminit. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            // Aggiungi diversi controlli ActiveX per dimostrare i vari tipi di persistenza
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);

            // Salva la cartella di lavoro con tutti i controlli ActiveX
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // Aggiungi un controllo ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                row,
                15,
                column,
                15,
                200,
                50
            );

            // Configura il controllo in base al tipo
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

            // Il tipo di persistenza è gestito internamente da Aspose.Cells durante il salvataggio
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



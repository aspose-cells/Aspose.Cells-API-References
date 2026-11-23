---
title: "Énumération ActiveXPersistenceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType enum. Représente la méthode de persistance pour persister un contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

Représente la méthode de persistance pour persister un contrôle ActiveX.

```csharp
public enum ActiveXPersistenceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| PropertyBag | `0` | Les données sont stockées sous forme de données XML. |
| Storage | `1` | Les données sont stockées sous forme de données binaires de stockage. |
| Stream | `2` | Les données sont stockées sous forme de données binaires de flux. |
| StreamInit | `3` | Les données sont stockées sous forme de données binaires de streaminit. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            // Ajoutez différents contrôles ActiveX pour démontrer les différents types de persistance
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);

            // Enregistrez le classeur avec tous les contrôles ActiveX
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // Ajoutez un contrôle ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                row,
                15,
                column,
                15,
                200,
                50
            );

            // Configurez le contrôle en fonction du type
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

            // Le type de persistance est géré en interne par Aspose.Cells lors de l'enregistrement
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



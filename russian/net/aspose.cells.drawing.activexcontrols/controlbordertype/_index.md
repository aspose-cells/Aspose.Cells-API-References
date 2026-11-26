---
title: "Перечисление ControlBorderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlBorderType. Представляет тип границы элемента управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlbordertype/
---
## ControlBorderType enumeration

Представляет тип границы ActiveX‑контрола.

```csharp
public enum ControlBorderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет границы. |
| Single | `1` | Одна строка. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;

    public class ControlBorderTypeDemo
    {
        public static void ControlBorderTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установить свойства для элемента управления ComboBox ActiveX
            comboBox.MaxLength = 100;
            comboBox.ListWidth = 150;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;
            comboBox.ColumnCount = 1;
            comboBox.ListRows = 5;
            comboBox.MatchEntry = ControlMatchEntryType.Complete;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow;
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
            comboBox.ListStyle = ControlListStyle.Plain;
            comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
            comboBox.IsEditable = true;
            comboBox.ShowColumnHeads = false;
            comboBox.IsDragBehaviorEnabled = false;
            comboBox.EnterFieldBehavior = true;
            comboBox.IsAutoWordSelected = false;
            comboBox.SelectionMargin = false;
            comboBox.Value = "Sample Text";
            comboBox.HideSelection = true;
            comboBox.ColumnWidths = 100;

            // Сохраните книгу
            workbook.Save("ControlBorderTypeExample.xlsx");
            workbook.Save("ControlBorderTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



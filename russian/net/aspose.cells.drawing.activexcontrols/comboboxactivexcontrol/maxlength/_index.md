---
title: "ComboBoxActiveXControl.MaxLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Получает и задает максимальное количество символов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/
---
## ComboBoxActiveXControl.MaxLength property

Получает и задает максимальное количество символов

```csharp
public int MaxLength { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установить свойство MaxLength и другие важные свойства
            comboBox.MaxLength = 10; // Restrict input to 10 characters
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;
            comboBox.Value = "Test";

            // Сохраните книгу
            workbook.Save("ComboBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



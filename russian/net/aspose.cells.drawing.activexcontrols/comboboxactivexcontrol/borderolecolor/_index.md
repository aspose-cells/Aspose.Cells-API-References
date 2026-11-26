---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Получает и задает OLE‑цвет фона"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Получает и задает ole‑цвет фона.

```csharp
public int BorderOleColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Настройте базовые свойства
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Продемонстрировать свойство BorderOleColor
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Задать примерный текст
            comboBox.Value = "Border Color Demo";

            // Сохраните книгу
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



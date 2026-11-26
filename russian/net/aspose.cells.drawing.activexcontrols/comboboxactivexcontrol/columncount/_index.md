---
title: "ComboBoxActiveXControl.ColumnCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Представляет количество столбцов, отображаемых в ComboBox или ListBox"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/
---
## ComboBoxActiveXControl.ColumnCount property

Представляет количество столбцов, отображаемых в ComboBox или ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Добавить ActiveX‑контрол ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установить свойство ColumnCount и другие свойства
            comboBox.ColumnCount = 1;
            comboBox.ListWidth = 100;
            comboBox.Value = "Apple;Banana;Cherry";

            // Сохраните книгу
            workbook.Save("ComboBoxColumnCountDemo.xlsx");

            Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



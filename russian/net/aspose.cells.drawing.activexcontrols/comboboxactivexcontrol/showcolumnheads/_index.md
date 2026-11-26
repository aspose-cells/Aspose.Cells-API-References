---
title: "ComboBoxActiveXControl.ShowColumnHeads"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает, отображаются ли заголовки столбцов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/
---
## ComboBoxActiveXControl.ShowColumnHeads property

Указывает, отображаются ли заголовки столбцов.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ComboBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListWidth = 100;
            
            // Добавьте примерные данные в ComboBox
            comboBox.ListFillRange = "A1:B3";
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Value1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Value2");

            // Продемонстрировать свойство ShowColumnHeads
            Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
            
            // Включить заголовки столбцов
            comboBox.ShowColumnHeads = true;
            Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
            
            // Отключить заголовки столбцов
            comboBox.ShowColumnHeads = false;
            Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);

            // Сохраните книгу
            workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



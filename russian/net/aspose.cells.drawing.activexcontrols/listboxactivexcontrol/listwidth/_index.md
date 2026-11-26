---
title: "ListBoxActiveXControl.ListWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Получает и задает ширину в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/listwidth/
---
## ListBoxActiveXControl.ListWidth property

Получает и задает ширину в единицах пунктов.

```csharp
public double ListWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ListBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                10, 10, 200, 100, 200, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство ListWidth
            listBox.ListWidth = 150;
            
            // Настройте базовые свойства
            listBox.ColumnCount = 2;
            listBox.ColumnWidths = 100; // Changed from string to double
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Red");
            worksheet.Cells["B2"].PutValue("Yellow");
            worksheet.Cells["B3"].PutValue("Orange");
            
            // Установить диапазон данных
            listBox.ListFillRange = "A1:B3";

            workbook.Save("ListBoxWidthDemo.xlsx");
            Console.WriteLine("ListBox with ListWidth=150 created successfully.");
        }
    }
}
```

### См. также

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



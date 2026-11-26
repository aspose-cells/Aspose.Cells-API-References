---
title: "ComboBox.DropDownLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBox. Получает или задает количество строк списка, отображаемых в выпадающей части комбобокса"
type: docs
url: /ru/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Получает или задает количество строк списка, отображаемых в раскрывающейся части комбобокса.

```csharp
public int DropDownLines { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте ComboBox с правильными параметрами
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Заполните ячейки листа элементами
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Свяжите комбобокс со значениями ячеек
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



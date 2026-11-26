---
title: "RadioButton.IsChecked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RadioButton. Указывает, отмечена ли радиокнопка или нет"
type: docs
url: /ru/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Указывает, отмечена ли радиокнопка.

```csharp
public bool IsChecked { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить радиокнопку на лист
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Установить текст радиокнопки
            radioButton.Text = "Option 1";
            
            // Изначально не отмечена
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Отметить радиокнопку
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Сохраните книгу
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### См. также

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



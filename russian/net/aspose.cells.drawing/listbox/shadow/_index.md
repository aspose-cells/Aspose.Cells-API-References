---
title: "ListBox.Shadow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBox. Указывает, имеет ли combobox 3D‑теневой эффект"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

Указывает, имеет ли комбобокс 3‑D затенение.

```csharp
public bool Shadow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить элементы списка
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Создать listbox и установить основные свойства
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Установить свойство тени
            listBox.Shadow = true;

            // Сохраните и перезагрузите для проверки
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### См. также

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



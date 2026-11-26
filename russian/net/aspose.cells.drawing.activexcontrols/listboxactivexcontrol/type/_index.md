---
title: "ListBoxActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Получает тип ActiveX‑элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/type/
---
## ListBoxActiveXControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте элемент управления ListBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            // Продемонстрировать свойство Type
            Console.WriteLine("Control Type: " + listBox.Type);
            
            // Установите некоторые свойства
            listBox.ScrollBars = ControlScrollBarType.BarsBoth;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Single;
            
            // Проверьте свойство Type
            if (listBox.Type == ControlType.ListBox)
            {
                Console.WriteLine("This is a ListBox control as expected");
            }
            
            // Сохраните книгу
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



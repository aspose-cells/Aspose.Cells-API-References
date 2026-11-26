---
title: "ListBoxActiveXControl.MatchEntry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBoxActiveXControl. Указывает, как ListBox или ComboBox ищут в списке при вводе пользователем"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/matchentry/
---
## ListBoxActiveXControl.MatchEntry property

Указывает, как ListBox или ComboBox ищет в списке при вводе пользователем.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");

            // Добавить элемент управления ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 0, 100, 80);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Настроить свойства ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.Value = "Apple;Banana;Cherry;Date";

            // Сохраните книгу
            workbook.Save("ListBoxMatchEntryDemo.xlsx");

            Console.WriteLine("ListBox with FirstLetter MatchEntry created successfully.");
        }
    }
}
```

### См. также

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



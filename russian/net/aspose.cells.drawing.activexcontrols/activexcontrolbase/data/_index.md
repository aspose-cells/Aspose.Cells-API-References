---
title: "ActiveXControlBase.Data"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает бинарные данные контролла"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Получает и задает двоичные данные элемента управления.

```csharp
public virtual byte[] Data { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.Drawing;

    public class ActiveXControlBasePropertyDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = "MyList";
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = ("A3:A7");
            list.Value = ("Apple");
            list.LinkedCell = ("A1");
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);

            // Отобразить начальную информацию свойства Data
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Изменить свойства элемента управления, влияющие на Data
            list.BackOleColor = 0xFF0000;

            // Отобразить обновленную информацию свойства Data
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Сохраните рабочую книгу, чтобы продемонстрировать сохранённые изменения
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



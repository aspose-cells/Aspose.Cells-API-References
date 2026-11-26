---
title: "ActiveXControl.IsLocked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Указывает, заблокированы ли данные в элементе управления для редактирования"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

Указывает, заблокированы ли данные в элементе управления для редактирования.

```csharp
public bool IsLocked { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsLockedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Разблокировать все столбцы, кроме первого
            Style style;
            StyleFlag flag;
            for (int i = 0; i <= 255; i++)
            {
                style = sheet.Cells.Columns[(byte)i].GetStyle();
                style.IsLocked = false;
                flag = new StyleFlag();
                flag.Locked = true;
                sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
            }

            // Заблокировать первый столбец
            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            // Добавить элемент управления ActiveX ComboBox
            Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                5, 0, 5, 0, 100, 20);

            // Установить свойства элемента управления ActiveX, включая IsLocked
            ComboBoxActiveXControl comboBox = 
                (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.IsLocked = false; // Demonstrate IsLocked property
            comboBox.IsVisible = true;
            comboBox.BorderStyle = ControlBorderType.None;

            // Защитить лист
            sheet.Protect(ProtectionType.All);

            // Сохраните книгу
            wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)



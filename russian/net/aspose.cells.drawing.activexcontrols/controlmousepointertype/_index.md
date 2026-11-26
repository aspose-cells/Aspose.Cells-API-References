---
title: "Перечисление ControlMousePointerType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType enum. Представляет тип значка, отображаемого в виде указателя мыши для элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Представляет тип значка, отображаемого в виде указателя мыши для элемента управления.

```csharp
public enum ControlMousePointerType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Стандартный указатель. |
| Arrow | `1` | Стрелка. |
| Cross | `2` | Указатель в виде перекрестия. |
| IBeam | `3` | Курсор I-образный. |
| SizeNESW | `6` | Двойная стрелка, указывающая на северо-восток и юго-запад. |
| SizeNS | `7` | Двойная стрелка, указывающая на север и юг. |
| SizeNWSE | `8` | Двойная стрелка, указывающая на северо-запад и юго-восток. |
| SizeWE | `9` | Двойная стрелка, указывающая на запад и восток. |
| UpArrow | `10` | Стрелка вверх. |
| HourGlass | `11` | Песочные часы. |
| NoDrop | `12` | \"Not\" символ (круг с диагональной линией) над перетаскиваемым объектом. |
| AppStarting | `13` | Стрелка с песочными часами. |
| Help | `14` | Стрелка с вопросительным знаком. |
| SizeAll | `15` | \"Size-all\" курсор (стрелки, указывающие на север, юг, восток и запад). |
| Custom | `99` | Использует значок, указанный свойством MouseIcon. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Преобразуйте ActiveXControl к ActiveXControlBase, чтобы получить доступ к его свойствам
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Установите тип указателя мыши для элемента управления
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Установите другие свойства для демонстрации
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Сохраните книгу
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Вывести результат.
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



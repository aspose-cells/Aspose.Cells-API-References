---
title: "Класс ActiveXControlBase"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ActiveXControls.ActiveXControlBase. Представляет элемент управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/
---
## ActiveXControlBase class

Представляет элемент управления ActiveX.

```csharp
public abstract class ActiveXControlBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Получает и задает ole‑цвет фона. |
| virtual [Data](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/data/) { get; } | Получает и задает двоичные данные элемента управления. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Получает и задает OLE‑цвет переднего плана. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Получает и задает высоту элемента управления в единицах точек. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Указывает, видим ли этот элемент управления. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Получает и задает связанную ячейку. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Получает и задает диапазон заполнения списка. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Получает и задает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Указывает, показывать ли тень. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Получает тип ActiveX‑элемента управления. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Получает и задает ширину элемента управления в единицах точек. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Получает объект [`Workbook`](./workbook/). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBaseDemo
    {
        public static void ActiveXControlBaseExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Установить свойства ActiveX‑контрола
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = "A1";
            control.ListFillRange = "A2:A10";

            // Сохраните книгу
            workbook.Save("ActiveXControlBaseExample.xlsx");
            workbook.Save("ActiveXControlBaseExample.pdf", SaveFormat.Pdf);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



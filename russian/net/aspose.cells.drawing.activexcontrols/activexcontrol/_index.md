---
title: "Класс ActiveXControl"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ActiveXControls.ActiveXControl. Представляет элемент управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Представляет элемент управления ActiveX.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Получает и задает ole‑цвет фона. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Получает и задает двоичные данные элемента управления. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Представляет шрифт элемента управления. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Получает и задает ole‑цвет переднего плана. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Получает и задает высоту элемента управления в пунктах. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Получает и задает режим выполнения по умолчанию редактора ввода (Input Method Editor) для элемента управления при получении фокуса. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Указывает, является ли элемент управления прозрачным. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Указывает, видим ли этот элемент управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Получает и задает связанную ячейку.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Получает и задает диапазон заполнения списка.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Получает и задает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Указывает, показывать ли тень.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Представляет способ выравнивания текста, используемого элементом управления. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Получает тип элемента управления ActiveX.(Наследуется от [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Получает и задает ширину элемента управления в единицах пунктов.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Получает объект [`Workbook`](../activexcontrolbase/workbook/).(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления RadioButton ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Установить свойства
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // Сохраните книгу
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



---
title: "Класс UnknownControl"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ActiveXControls.UnknownControl. Неизвестный элемент управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Неизвестный элемент управления.

```csharp
public class UnknownControl : ActiveXControl
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Получает и задает ole‑цвет фона. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Получает и задает двоичные данные элемента управления. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Представляет шрифт элемента управления. (Унаследовано от [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Получает и задает ole‑цвет переднего плана. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Получает и задает высоту элемента управления в пунктах. (Унаследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Получает и задает режим выполнения по умолчанию редактора ввода (Input Method Editor) для элемента управления при получении им фокуса. (Унаследовано от [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. (Унаследовано от [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. (Унаследовано от [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Указывает, заблокированы ли данные в элементе управления для редактирования. (Унаследовано от [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Указывает, является ли элемент управления прозрачным.(Наследовано от [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Указывает, видим ли этот элемент управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Получает и задает связанную ячейку.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Получает и задает диапазон заполнения списка.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Получает и задает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Указывает, показывать ли тень.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Представляет способ выравнивания текста, используемого элементом управления.(Наследовано от [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | Получает тип ActiveX‑элемента управления. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Получает и задает ширину элемента управления в единицах пунктов.(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Получает объект [`Workbook`](../activexcontrolbase/workbook/).(Наследовано от [`ActiveXControlBase`](../activexcontrolbase/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | Получает связанные данные. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте неизвестный элемент управления ActiveX на лист
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Получите экземпляр UnknownControl из фигуры
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Сохраните книгу
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)



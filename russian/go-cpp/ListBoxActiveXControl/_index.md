---
title: "Класс ListBoxActiveXControl"
linktitle: "ListBoxActiveXControl"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ListBoxActiveXControl. Инкапсулирует объект, представляющий listboxactivexcontrol в Go."
type: docs
weight: 200
url: /ru/go-cpp/listboxactivexcontrol/
---

## ListBoxActiveXControl class

Представляет элемент управления ListBox ActiveX.

```go

type ListBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewListBoxActiveXControl](./newlistboxactivexcontrol/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetType](./gettype/) | Получает тип элемента управления ActiveX. |
| [GetScrollBars](./getscrollbars/) | Указывает, определяет, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни одного. |
| [SetScrollBars](./setscrollbars/) | Указывает, определяет, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни одного. |
| [GetListWidth](./getlistwidth/) | Получает и задает ширину в единицах пунктов. |
| [SetListWidth](./setlistwidth/) | Получает и задает ширину в единицах пунктов. |
| [GetBoundColumn](./getboundcolumn/) | Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle). |
| [SetBoundColumn](./setboundcolumn/) | Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle). |
| [GetTextColumn](./gettextcolumn/) | Представляет столбец в ComboBox или ListBox, отображаемый пользователю. |
| [SetTextColumn](./settextcolumn/) | Представляет столбец в ComboBox или ListBox, отображаемый пользователю. |
| [GetColumnCount](./getcolumncount/) | Представляет количество столбцов, отображаемых в ComboBox или ListBox. |
| [SetColumnCount](./setcolumncount/) | Представляет количество столбцов, отображаемых в ComboBox или ListBox. |
| [GetMatchEntry](./getmatchentry/) | Указывает, как ListBox или ComboBox ищут в списке по мере ввода пользователем. |
| [SetMatchEntry](./setmatchentry/) | Указывает, как ListBox или ComboBox ищут в списке по мере ввода пользователем. |
| [GetListStyle](./getliststyle/) | Получает и задает визуальное оформление. |
| [SetListStyle](./setliststyle/) | Получает и задает визуальное оформление. |
| [GetSelectionType](./getselectiontype/) | Указывает, разрешает ли элемент управления множественный выбор. |
| [SetSelectionType](./setselectiontype/) | Указывает, разрешает ли элемент управления множественный выбор. |
| [GetValue](./getvalue/) | Получает и задает значение элемента управления. |
| [SetValue](./setvalue/) | Получает и задает значение элемента управления. |
| [GetBorderStyle](./getborderstyle/) | Получает и задает тип границы, используемой элементом управления. |
| [SetBorderStyle](./setborderstyle/) | Получает и задает тип границы, используемой элементом управления. |
| [GetBorderOleColor](./getborderolecolor/) | Получает и задает OLE‑цвет фона. |
| [SetBorderOleColor](./setborderolecolor/) | Получает и задает OLE‑цвет фона. |
| [GetSpecialEffect](./getspecialeffect/) | Получает и задает специальный эффект элемента управления. |
| [SetSpecialEffect](./setspecialeffect/) | Получает и задает специальный эффект элемента управления. |
| [GetShowColumnHeads](./getshowcolumnheads/) | Указывает, отображаются ли заголовки столбцов. |
| [SetShowColumnHeads](./setshowcolumnheads/) | Указывает, отображаются ли заголовки столбцов. |
| [GetIntegralHeight](./getintegralheight/) | Указывает, будет ли элемент управления показывать только полные строки текста, не отображая частичные строки. |
| [SetIntegralHeight](./setintegralheight/) | Указывает, будет ли элемент управления показывать только полные строки текста, не отображая частичные строки. |
| [GetColumnWidths](./getcolumnwidths/) | Получает и задает ширину столбца. |
| [SetColumnWidths](./setcolumnwidths/) | Получает и задает ширину столбца. |
| [IsEnabled](./isenabled/) | Указывает, может ли элемент управления получать фокус и реагировать на генерируемые пользователем события. |
| [SetIsEnabled](./setisenabled/) | Указывает, может ли элемент управления получать фокус и реагировать на генерируемые пользователем события. |
| [IsLocked](./islocked/) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [SetIsLocked](./setislocked/) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [IsTransparent](./istransparent/) | Указывает, является ли элемент управления прозрачным. |
| [SetIsTransparent](./setistransparent/) | Указывает, является ли элемент управления прозрачным. |
| [GetIMEMode](./getimemode/) | Получает и задает режим выполнения по умолчанию для Input Method Editor элемента управления при получении им фокуса. |
| [SetIMEMode](./setimemode/) | Получает и задает режим выполнения по умолчанию для Input Method Editor элемента управления при получении им фокуса. |
| [GetFont](./getfont/) | Представляет шрифт элемента управления. |
| [GetTextAlign](./gettextalign/) | Представляет способ выравнивания текста, используемого элементом управления. |
| [SetTextAlign](./settextalign/) | Представляет способ выравнивания текста, используемого элементом управления. |
| [GetData](./getdata/) | Получает и задает двоичные данные элемента управления. |
| [IsAutoSize](./isautosize/) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [SetIsAutoSize](./setisautosize/) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [GetWorkbook](./getworkbook/) | Получает объект Workbook. |
| [GetMouseIcon](./getmouseicon/) | Получает и задает пользовательскую иконку, отображаемую в виде указателя мыши для элемента управления. |
| [SetMouseIcon](./setmouseicon/) | Получает и задает пользовательскую иконку, отображаемую в виде указателя мыши для элемента управления. |
| [GetMousePointer](./getmousepointer/) | Получает и задает тип иконки, отображаемой в виде указателя мыши для элемента управления. |
| [SetMousePointer](./setmousepointer/) | Получает и задает тип иконки, отображаемой в виде указателя мыши для элемента управления. |
| [GetLinkedCell](./getlinkedcell/) | Получает и задает связанную ячейку. |
| [SetLinkedCell](./setlinkedcell/) | Получает и задает связанную ячейку. |
| [GetListFillRange](./getlistfillrange/) | Получает и задает диапазон заполнения списка. |
| [SetListFillRange](./setlistfillrange/) | Получает и задает диапазон заполнения списка. |
| [GetWidth](./getwidth/) | Получает и задает ширину элемента управления в пунктах. |
| [SetWidth](./setwidth/) | Получает и задает ширину элемента управления в пунктах. |
| [GetHeight](./getheight/) | Получает и задает высоту элемента управления в пунктах. |
| [SetHeight](./setheight/) | Получает и задает высоту элемента управления в пунктах. |
| [GetForeOleColor](./getforeolecolor/) | Получает и задает OLE‑цвет переднего плана. |
| [SetForeOleColor](./setforeolecolor/) | Получает и задает OLE‑цвет переднего плана. |
| [GetBackOleColor](./getbackolecolor/) | Получает и задает OLE‑цвет фона. |
| [SetBackOleColor](./setbackolecolor/) | Получает и задает OLE‑цвет фона. |
| [IsVisible](./isvisible/) | Указывает, видим ли этот элемент управления. |
| [SetIsVisible](./setisvisible/) | Указывает, видим ли этот элемент управления. |
| [GetShadow](./getshadow/) | Указывает, показывать ли тень. |
| [SetShadow](./setshadow/) | Указывает, показывать ли тень. |

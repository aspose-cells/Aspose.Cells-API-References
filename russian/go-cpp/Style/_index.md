---
title: "Класс Style"
linktitle: "Style"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Style. Инкапсулирует объект, представляющий стиль в Go."
type: docs
weight: 200
url: /ru/go-cpp/style/
---

## Style class

Представляет стиль отображения Excel‑документа, такой как шрифт, цвет, выравнивание, граница и т.д. Объект Style содержит все атрибуты стиля (шрифт, числовой формат, выравнивание и т.п.) в виде свойств.

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Получает и задает цвет фоновой темы. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Получает и задает цвет фоновой темы. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Получает и задает цвет передней темы. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Получает и задает цвет передней темы. |
| [GetName](./getname/) | Получает или задает имя стиля. |
| [SetName](./setname/) | Получает или задает имя стиля. |
| [GetPattern](./getpattern/) | Получает или задает тип фонового узора ячейки. |
| [SetPattern](./setpattern/) | Получает или задает тип фонового узора ячейки. |
| [SetPatternColor](./setpatterncolor/) | Задает цвет фона. |
| [GetBorders](./getborders/) | Получает BorderCollection стиля. |
| [GetBackgroundColor](./getbackgroundcolor/) | Получает или задает фоновый цвет стиля. |
| [SetBackgroundColor](./setbackgroundcolor/) | Получает или задает фоновый цвет стиля. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | Получает и задает цвет фона с 32‑битным значением ARGB. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | Получает и задает цвет фона с 32‑битным значением ARGB. |
| [GetForegroundColor](./getforegroundcolor/) | Получает или задает передний цвет стиля. |
| [SetForegroundColor](./setforegroundcolor/) | Получает или задает передний цвет стиля. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | Получает и задает передний цвет с 32‑битным значением ARGB. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | Получает и задает передний цвет с 32‑битным значением ARGB. |
| [Copy](./copy/) | Копирует данные из другого объекта стиля. |
| [GetHasBorders](./gethasborders/) | Проверяет, установлены ли границы для стиля. |
| [GetParentStyle](./getparentstyle/) | Получает родительский стиль этого стиля. |
| [Update](./update/) | Применить именованный стиль к стилям ячеек, использующих этот именованный стиль. Это работает как нажатие кнопки "ok" после завершения изменения стиля. Применяется только к именованному стилю. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Указывает, следует ли применять форматирование чисел. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Указывает, следует ли применять форматирование чисел. |
| [IsFontApplied](./isfontapplied/) | Указывает, следует ли применять форматирование шрифта. |
| [SetIsFontApplied](./setisfontapplied/) | Указывает, следует ли применять форматирование шрифта. |
| [IsAlignmentApplied](./isalignmentapplied/) | Указывает, следует ли применять форматирование выравнивания. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Указывает, следует ли применять форматирование выравнивания. |
| [IsBorderApplied](./isborderapplied/) | Указывает, следует ли применять форматирование границ. |
| [SetIsBorderApplied](./setisborderapplied/) | Указывает, следует ли применять форматирование границ. |
| [IsFillApplied](./isfillapplied/) | Указывает, следует ли применять форматирование заливки. |
| [SetIsFillApplied](./setisfillapplied/) | Указывает, следует ли применять форматирование заливки. |
| [IsProtectionApplied](./isprotectionapplied/) | Указывает, следует ли применять форматирование защиты. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Указывает, следует ли применять форматирование защиты. |
| [IsModified](./ismodified/) | Проверяет, были ли изменены указанные свойства стиля. Используется для стилей ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке. |
| [Equals](./equals/) | Определяет, равны ли два экземпляра Style. |
| [GetHashCode](./gethashcode/) | Служит хеш‑функцией для объекта Style. |
| [GetIndentLevel](./getindentlevel/) | Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250. |
| [SetIndentLevel](./setindentlevel/) | Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250. |
| [GetFont](./getfont/) | Получает объект Font. |
| [GetRotationAngle](./getrotationangle/) | Представляет угол поворота текста. |
| [SetRotationAngle](./setrotationangle/) | Представляет угол поворота текста. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Получает или задает тип горизонтального выравнивания текста в ячейке. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Получает или задает тип горизонтального выравнивания текста в ячейке. |
| [GetVerticalAlignment](./getverticalalignment/) | Получает или задает тип вертикального выравнивания текста в ячейке. |
| [SetVerticalAlignment](./setverticalalignment/) | Получает или задает тип вертикального выравнивания текста в ячейке. |
| [IsTextWrapped](./istextwrapped/) | Получает или задает значение, указывающее, переносится ли текст в ячейке. |
| [SetIsTextWrapped](./setistextwrapped/) | Получает или задает значение, указывающее, переносится ли текст в ячейке. |
| [GetNumber](./getnumber/) | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [SetNumber](./setnumber/) | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Устанавливает границы стиля. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Устанавливает границы стиля. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Установить контурные границы |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Установить контурные границы |
| [IsLocked](./islocked/) | Получает или задает значение, указывающее, может ли ячейка быть изменена. |
| [SetIsLocked](./setislocked/) | Получает или задает значение, указывающее, может ли ячейка быть изменена. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Устанавливает строку пользовательского числового формата ячейки. |
| [GetCustom](./getcustom/) | Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не установлен (например, числовой формат встроенный), будет возвращена пустая строка "". |
| [SetCustom_String](./setcustom_string/) | Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не установлен (например, числовой формат встроенный), будет возвращена пустая строка "". |
| [GetCultureCustom](./getculturecustom/) | Получает и задает зависящую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу. |
| [SetCultureCustom](./setculturecustom/) | Получает и задает зависящую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу. |
| [GetInvariantCustom](./getinvariantcustom/) | Получает независимую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу. |
| [IsFormulaHidden](./isformulahidden/) | Представляет, будет ли формула скрыта, когда лист защищён. |
| [SetIsFormulaHidden](./setisformulahidden/) | Представляет, будет ли формула скрыта, когда лист защищён. |
| [GetShrinkToFit](./getshrinktofit/) | Представляет, будет ли текст автоматически уменьшаться, чтобы поместиться в доступную ширину столбца. |
| [SetShrinkToFit](./setshrinktofit/) | Представляет, будет ли текст автоматически уменьшаться, чтобы поместиться в доступную ширину столбца. |
| [GetTextDirection](./gettextdirection/) | Представляет порядок чтения текста. |
| [SetTextDirection](./settextdirection/) | Представляет порядок чтения текста. |
| [IsJustifyDistributed](./isjustifydistributed/) | Указывает, следует ли использовать выравнивание по ширине или распределённое выравнивание ячеек в последней строке текста. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Указывает, следует ли использовать выравнивание по ширине или распределённое выравнивание ячеек в последней строке текста. |
| [GetQuotePrefix](./getquoteprefix/) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [SetQuotePrefix](./setquoteprefix/) | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [IsGradient](./isgradient/) | Указывает, является ли заливка ячейки градиентным шаблоном. |
| [SetIsGradient](./setisgradient/) | Указывает, является ли заливка ячейки градиентным шаблоном. |
| [SetTwoColorGradient](./settwocolorgradient/) | Устанавливает указанную заливку как двухцветный градиент. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Получить настройку двухцветного градиента. |
| [IsPercent](./ispercent/) | Указывает, является ли числовой формат процентным. |
| [IsDateTime](./isdatetime/) | Указывает, является ли числовой формат датой. |
| [IsCheckBox](./ischeckbox/) | Указывает, является ли это стилем флажка. |
| [SetIsCheckBox](./setischeckbox/) | Указывает, является ли это стилем флажка. |
| [ToJson](./tojson/) | Преобразовать стиль в структуру данных JSON. |
| [GetLeftBorder](./getleftborder/) | Получает левую границу. |
| [GetRightBorder](./getrightborder/) | Получает правую границу. |
| [GetTopBorder](./gettopborder/) | Получает верхнюю границу. |
| [GetBottomBorder](./getbottomborder/) | Получает нижнюю границу. |

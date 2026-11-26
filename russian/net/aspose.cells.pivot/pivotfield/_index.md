---
title: "Класс PivotField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotField. Представляет поле в отчете сводной таблицы."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Представляет поле в отчете PivotTable.

```csharp
public class PivotField : IDisposable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowDraggingToColumn](../../aspose.cells.pivot/pivotfield/allowdraggingtocolumn/) { get; set; } | Указывает, может ли указанный поле быть перетянуто в область столбцов. Значение по умолчанию — true. |
| [AllowDraggingToData](../../aspose.cells.pivot/pivotfield/allowdraggingtodata/) { get; set; } | Указывает, может ли указанный поле быть перетянуто в область значений. Значение по умолчанию — true. |
| [AllowDraggingToPage](../../aspose.cells.pivot/pivotfield/allowdraggingtopage/) { get; set; } | Указывает, может ли указанный поле быть перетянуто в область страниц. Значение по умолчанию — true. |
| [AllowDraggingToRow](../../aspose.cells.pivot/pivotfield/allowdraggingtorow/) { get; set; } | Указывает, может ли указанный поле быть перетянуто в область строк. Значение по умолчанию — true. |
| [AllowRemovingFromView](../../aspose.cells.pivot/pivotfield/allowremovingfromview/) { get; set; } | Указывает, может ли данное поле сводки быть удалено из представления сводной таблицы. Значение по умолчанию — true. |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | (**Устаревший.**) Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | (**Устаревший.**) Представляет индекс автоматически отображаемого поля. -1 означает сам PivotField. Это должен быть индекс полей данных. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | (**Устаревший.**) Представляет индекс поля, которое автоматически сортируется. -1 означает сам PivotField, остальные означают позицию полей данных. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Представляет индекс в исходных полях сводной таблицы. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Получает или задает текущий отображаемый элемент страницы для этого поля сводной таблицы (только поле страницы). |
| [CurrentPageItemText](../../aspose.cells.pivot/pivotfield/currentpageitemtext/) { get; set; } | Получает текст отображения текущего элемента страницы для этого поля сводной таблицы (только поле страницы). |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Представляет отображаемое имя поля сводной таблицы в представлении сводной таблицы. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | (**Устаревший.**) Указывает, может ли указанное поле быть перетащено в область столбцов. Значение по умолчанию — true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | (**Устаревший.**) Указывает, может ли указанное поле быть перетащено в область значений. Значение по умолчанию — true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | (**Устаревший.**) Указывает, может ли это поле сводной таблицы быть удалено из представления сводной таблицы. Значение по умолчанию — true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | (**Устаревший.**) Указывает, может ли указанное поле быть перетащено в область страниц. Значение по умолчанию — true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | (**Устаревший.**) Указывает, может ли указанное поле быть перетащено в область строк. Значение по умолчанию — true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Представляет функцию, используемую для суммирования этого поля данных сводной таблицы. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Получает настройки группировки поля сводной таблицы. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | (**Устаревший.**) Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | (**Устаревший.**) Указывает, сортируются ли элементы этого поля сводной таблицы автоматически по возрастанию. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | (**Устаревший.**) Указывает, отображается ли указанное поле сводной таблицы автоматически. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | (**Устаревший.**) Указывает, сортируются ли элементы этого поля сводной таблицы автоматически. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию — true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Указывает, является ли это поле сводной таблицы вычисляемым полем. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | Указывает, следует ли включать новые элементы в поле при ручной фильтрации. Значение по умолчанию — false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | Указывает, следует ли вставлять разрывы страниц после каждого элемента. Значение по умолчанию — false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | Указывает, можно ли выбрать несколько элементов в поле страницы. Значение по умолчанию — false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | Указывает, следует ли повторять метки поля в области строк или столбцов. Значение по умолчанию — false. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) Указывает, представляет ли это поле поля значений. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | Указывает, представляет ли это поле поле значений. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | (**Obsolete.**) Получает количество базовых элементов в этом сводном поле. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Получить все метки элементов сводной таблицы в этом поле. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Представляет имя PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | (**Obsolete.**) Указывает, является ли операция сортировки, которая будет применена к этому сводному полю, автоматической сортировкой или простой сортировкой данных. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Представляет встроенный формат отображения чисел и дат. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Представляет пользовательский формат отображения чисел и дат. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Получить оригинальные базовые элементы; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Получает элементы сводного поля. |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Представляет индекс `PivotField` в области. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | Указывает область сводной таблицы, в которой отображается это поле. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | (**Obsolete.**) Указывает, следует ли отображать метки следующего поля в той же колонке в представлении Pivot Table. Только для полей строк. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivotfield/showincompactform/) { get; set; } | Получает или задает значение, указывающее, использует ли это поле строки компактный макет. Применяется только к полям строк. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Получает или задает значение, указывающее, использует ли это поле строки схематический макет. Применяется только к полям строк. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | Указывает, отображать ли промежуточные итоги вверху или внизу элементов. |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | Получает настройки отображения значений, когда используется вычисление ShowDataAs. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | Получает все настройки автоматической сортировки |
| [Subtotals](../../aspose.cells.pivot/pivotfield/subtotals/) { get; set; } | Получает или задает промежуточные итоги поля. Только для строкового или столбцового сводного поля. |
| [Top10AutoShowSettings](../../aspose.cells.pivot/pivotfield/top10autoshowsettings/) { get; } | Получает настройки Top 10 AutoShow для сводного поля. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Добавить элемент вычисляемой формулы в сводное поле. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | Очищает настройки фильтра для этого сводного поля. |
| [Dispose](../../aspose.cells.pivot/pivotfield/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | Фильтрует по датам значений строкового или столбцового сводного поля. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | Фильтрует по заголовкам строки или столбца сводного поля. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | Фильтрует по значениям данных сводного поля. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | Фильтрует по значениям данных сводного поля. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) Получить строку формулы указанного вычисляемого поля. |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | Получает все фильтры сводки, применённые к этому полю сводки. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | Получает формулу вычисляемого поля. Работает только для вычисляемого поля. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | Получает максимальное значение этого поля. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | Получает максимальное значение этого поля. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Получает фильтр сводки поля сводки по типу |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) Получает фильтры сводки поля сводки |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Указывает, следует ли показывать указанный промежуточный итог для этого поля сводки. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group)() | Автоматически группировать поле. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group_1)(PivotFieldGroupOptions) | Группирует поле сводки с параметрами. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | (**Obsolete.**) Пользовательская группировка поля. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(DiscreteGroupItem[], bool) | (**Obsolete.**) Пользовательская группировка поля. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_7)(double, bool) | (**Obsolete.**) Автоматически группировать поле с интервалом |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(PivotGroupByType[], double, bool) | (**Obsolete.**) Автоматически группировать поле с внутренним параметром |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(double, double, double, bool) | (**Obsolete.**) Группировать файл по номеру. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(DateTime, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Группировать файл по типам группировки даты. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, double, bool, double, double, bool) | (**Obsolete.**) Группировать файл по номеру. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Группировать файл по типам группировки даты. |
| [HideAllDetails](../../aspose.cells.pivot/pivotfield/hidealldetails/)() | Скрывает все детали каждого элемента сводки. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | (**Obsolete.**) Устанавливает, скрыты ли детали всех PivotItems в поле сводки. То есть сворачивает/разворачивает это поле. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | (**Obsolete.**) Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | (**Obsolete.**) Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | (**Obsolete.**) Устанавливает, скрыты ли детали конкретного PivotItem в поле сводки. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | (**Obsolete.**) Инициализировать элементы сводки поля сводки |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | (**Obsolete.**) Указывает, скрыт ли конкретный PivotItem. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | (**Obsolete.**) Указывает, следует ли скрыть детали конкретного PivotItem. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Устанавливает, как подсчитывать промежуточный итог указанного поля. |
| [ShowAllDetails](../../aspose.cells.pivot/pivotfield/showalldetails/)() | Показать все детали каждого элемента сводки. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_1)(PivotShowValuesAsType, int, int) | Устанавливает вычисление "Show Values As" для этого поля сводки. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_2)(PivotShowValuesAsType, string, string) | Настраивает вычисление "Show Values As" для этого поля данных. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | (**Obsolete.**) Показывает значения поля данных в другом формате отображения, когда используется вычисление ShowDataAs. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder) | Сортирует это сводное поле. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int) | (**Obsolete.**) Сортирует это сводное поле. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_3)(SortOrder, int, string) | Сортирует это сводное поле. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_2)(SortOrder, int, PivotLineType, string) | (**Obsolete.**) Сортирует это сводное поле. |
| [Top10AutoShow](../../aspose.cells.pivot/pivotfield/top10autoshow/)(bool, bool, int, int) | Настраивает параметры Top10 AutoShow для этого сводного поля. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Разгруппировать сводное поле. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить некоторые данные в лист
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Добавьте сводную таблицу на лист.
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Установить стиль pivot table
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Получить доступ к полю строки
            PivotField rowField = pivotTable.RowFields[0];

            // Установить свойства PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.ShowValuesAs(PivotFieldDataDisplayFormat.PercentageOfTotal, 0, PivotItemPositionType.Next, 0);
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



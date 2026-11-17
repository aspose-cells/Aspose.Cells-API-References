---
title: "PivotField Класс"
linktitle: "PivotField"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PivotField класс. Инкапсулирует объект, представляющий pivotfield в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotfield/
---

## PivotField class

Представляет поле в отчёте PivotTable.

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | Получает элементы pivot field |
| [GetMaxValue](./getmaxvalue/) | Получает максимальное значение этого поля. |
| [GetMinValue](./getminvalue/) | Получает максимальное значение этого поля. |
| [GetGroupSettings](./getgroupsettings/) | Получает настройки группировки pivot field. |
| [InitPivotItems](./initpivotitems/) | Инициализирует элементы pivot field |
| [Group](./group/) | Автоматически группирует поле. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Группирует pivot field с параметрами. |
| [GroupBy](./groupby/) | Пользовательская группировка поля. |
| [Ungroup](./ungroup/) | Разгруппировать pivot field. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Получает фильтр сводного поля по типу |
| [GetFilters](./getfilters/) | Получает все фильтры сводного поля, применённые к этому полю. |
| [ClearFilter](./clearfilter/) | Очищает настройки фильтра для этого сводного поля. |
| [FilterTop10](./filtertop10/) | Фильтрует по значениям поля данных pivot. |
| [FilterByValue](./filterbyvalue/) | Фильтрует по значениям поля данных pivot. |
| [FilterByLabel](./filterbylabel/) | Фильтрует по подписям строкового или столбцового поля pivot. |
| [FilterByDate](./filterbydate/) | Фильтрует по датам значений строкового или столбцового сводного поля. |
| [IsCalculatedField](./iscalculatedfield/) | Указывает, является ли это сводное поле вычисляемым полем. |
| [GetFormula](./getformula/) | Получает формулу вычисляемого поля. Работает только для вычисляемых полей. |
| [IsValuesField](./isvaluesfield/) | Указывает, представляет ли это поле поле значений. |
| [GetBaseIndex](./getbaseindex/) | Представляет индекс в исходных сводных полях. |
| [SetBaseIndex](./setbaseindex/) | Представляет индекс в исходных сводных полях. |
| [GetPosition](./getposition/) | Представляет индекс PivotField в области. |
| [GetRegionType](./getregiontype/) | Указывает область сводной таблицы, в которой отображается это поле. |
| [GetName](./getname/) | Представляет имя PivotField. |
| [SetName](./setname/) | Представляет имя PivotField. |
| [GetDisplayName](./getdisplayname/) | Представляет отображаемое имя сводного поля в представлении сводной таблицы. |
| [SetDisplayName](./setdisplayname/) | Представляет отображаемое имя сводного поля в представлении сводной таблицы. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Устанавливает способ подсчёта промежуточных итогов для указанного поля. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Указывает, показывать ли указанный промежуточный итог для этого сводного поля. |
| [GetSubtotals](./getsubtotals/) | Получает или задаёт промежуточные итоги поля. Только для строковых или столбцовых сводных полей. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Получает или задаёт промежуточные итоги поля. Только для строковых или столбцовых сводных полей. |
| [IsAutoSubtotals](./isautosubtotals/) | Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию true. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Указывает, отображает ли указанное поле автоматические промежуточные итоги. По умолчанию true. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Указывает, можно ли перетаскивать указанное поле в область строк. Значение по умолчанию — true. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Указывает, можно ли перетаскивать указанное поле в область столбцов. Значение по умолчанию — true. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Указывает, можно ли перетаскивать указанное поле в область страниц. Значение по умолчанию — true. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Указывает, можно ли удалить это сводное поле из представления PivotTable. Значение по умолчанию — true. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Указывает, можно ли удалить это сводное поле из представления PivotTable. Значение по умолчанию — true. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Указывает, можно ли перетаскивать указанное поле в область значений. Значение по умолчанию — true. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Указывает, можно ли выбирать несколько элементов в поле страниц. Значение по умолчанию — false. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Указывает, можно ли выбирать несколько элементов в поле страниц. Значение по умолчанию — false. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Указывает, повторять ли метки поля в области. Значение по умолчанию — false. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Указывает, повторять ли метки поля в области. Значение по умолчанию — false. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Указывает, включать ли новые элементы в поле при ручном фильтре. Значение по умолчанию — false. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Указывает, включать ли новые элементы в поле при ручном фильтре. Значение по умолчанию — false. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Указывает, вставлять ли разрывы страниц после каждого элемента. Значение по умолчанию — false. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Указывает, вставлять ли разрывы страниц после каждого элемента. Значение по умолчанию — false. |
| [GetShowAllItems](./getshowallitems/) | Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false. |
| [SetShowAllItems](./setshowallitems/) | Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false. |
| [SortBy_SortOrder](./sortby_sortorder/) | Сортирует это поле сводной таблицы. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Сортирует это поле сводной таблицы. |
| [GetSortSetting](./getsortsetting/) | Получает все настройки автоматической сортировки |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Получает настройки Top 10 AutoShow для поля сводной таблицы. |
| [Top10AutoShow](./top10autoshow/) | Настраивает параметры Top10 AutoShow для этого поля сводной таблицы. |
| [GetFunction](./getfunction/) | Представляет функцию, используемую для суммирования этого поля данных PivotTable. |
| [SetFunction](./setfunction/) | Представляет функцию, используемую для суммирования этого поля данных PivotTable. |
| [ShowValuesAs](./showvaluesas/) | Отображает значения поля данных в другом формате отображения, когда используется вычисление ShowDataAs. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Получает настройки отображения значений, когда используется вычисление ShowDataAs. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Представляет текущий выбранный элемент страницы поля страницы для фильтрации данных. Действительно только для полей страниц. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Представляет текущий выбранный элемент страницы поля страницы для фильтрации данных. Действительно только для полей страниц. |
| [GetInsertBlankRow](./getinsertblankrow/) | Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк. |
| [SetInsertBlankRow](./setinsertblankrow/) | Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов, когда ShowInOutlineForm равно true, затем |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Указывает, следует ли отображать промежуточные итоги вверху или внизу элементов, когда ShowInOutlineForm равно true, затем |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Указывает, следует ли размещать это поле в виде контура в представлении Pivot Table. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Указывает, следует ли размещать это поле в виде контура в представлении Pivot Table. |
| [GetNumber](./getnumber/) | Представляет встроенный формат отображения чисел и дат. |
| [SetNumber](./setnumber/) | Представляет встроенный формат отображения чисел и дат. |
| [Get_NumberFormat](./get_numberformat/) | Представляет пользовательский формат отображения чисел и дат. |
| [SetNumberFormat](./setnumberformat/) | Представляет пользовательский формат отображения чисел и дат. |
| [HideAllDetails](./hidealldetails/) | Скрывает все детали |
| [ShowAllDetails](./showalldetails/) | Показать все детали |
| [GetItems](./getitems/) | Получить все метки элементов сводной таблицы в этом поле. |
| [GetOriginalItems](./getoriginalitems/) | Получить исходные базовые элементы; |
| [AddCalculatedItem](./addcalculateditem/) | Добавить вычисляемый элемент формулы в поле сводной таблицы. |
| [GetShowCompact](./getshowcompact/) | Указывает, следует ли отображать метки следующего поля в том же столбце в представлении Pivot Table |
| [SetShowCompact](./setshowcompact/) | Указывает, следует ли отображать метки следующего поля в том же столбце в представлении Pivot Table |

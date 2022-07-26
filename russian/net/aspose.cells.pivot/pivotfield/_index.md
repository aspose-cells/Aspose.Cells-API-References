---
title: PivotField
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет поле в отчете сводной таблицы.
type: docs
weight: 4530
url: /ru/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Представляет поле в отчете сводной таблицы.

```csharp
public class PivotField
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Представляет количество верхних или нижних элементов , которые автоматически отображаются в указанном поле сводной таблицы. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Представляет индекс поля автопоказа. -1 означает сам PivotField. Это должен быть индекс полей данных. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Представляет индекс поля автоматической сортировки. -1 означает само PivotField, остальные означают положение полей данных. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Представляет базовое поле для пользовательского расчета. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Представляет индекс PivotField в базовых PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Представляет элемент в базовом поле для пользовательского расчета. Допустимо только для полей данных. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Представляет элемент в базовом поле для пользовательского расчета. Допустимо только для полей данных. Поскольку PivotItemPosition.Custom предназначен только для чтения, если вам нужно установить PivotItemPosition.Custom, установите атрибут PivotField.BaseItemIndex. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Представляет текущий элемент страницы, отображаемый для поля страницы (действительно только для полей страницы). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Представляет, как отображать значения, содержащиеся в поле данных. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Представляет отображаемое имя PivotField. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Указывает, можно ли перетащить указанное поле в позицию столбца. Значение по умолчанию — true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Указывает, можно ли перетащить указанное поле в позицию данных. Значение по умолчанию — true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Указывает, можно ли перетащить указанное поле в позицию скрытия. Значение по умолчанию — true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Указывает, можно ли перетаскивать указанное поле на позицию страницы. Значение по умолчанию — true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Указывает, можно ли перетащить указанное поле в позицию строки. Значение по умолчанию — true. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Представляет функцию, используемую для суммирования поля данных сводной таблицы. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Указывает, вставляется ли пустая строка после каждого элемента. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Указывает, сортируется ли указанное поле сводной таблицы автоматически по возрастанию. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Указывает, отображается ли указанное поле сводной таблицы автоматически. Допустимо только для Excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Указывает, сортируется ли указанное поле сводной таблицы автоматически. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Указывает, отображаются ли в указанном поле автоматические промежуточные итоги. Значение по умолчанию — true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Указывает, является ли указанное поле сводной таблицы вычисляемым полем. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | указывает, может ли поле включать новые элементы в ручном filter Значение по умолчанию — false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | указывает, может ли поле вставлять разрывы страниц между элементами вставлять разрывы страниц после каждого элемента Значение по умолчанию — false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | указывает, может ли поле иметь несколько элементов , выбранных на странице field Значение по умолчанию — false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | указывает, может ли поле повторять элементы labels Значение по умолчанию — false. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Получает количество базовых элементов в этом сводном поле. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Получить все базовые предметы; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Представляет имя PivotField. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Представляет встроенный формат отображения чисел и дат. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Представляет пользовательский формат отображения чисел и дат. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Получить исходные базовые предметы; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Получает элементы сводки поля сводки |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Представляет индекс PivotField в PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Получает диапазон группы сводного поля |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Указывает, отображаются ли все элементы в отчете сводной таблицы, , даже если они не содержат сводных данных. показывать элементы без данных Значение по умолчанию — false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Указывает, отображать ли метки из следующего поля в том же столбце сводной таблицы view |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Указывает, размещается ли это поле в виде схемы в сводной таблице view |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | , когда ShowInOutlineForm имеет значение true, промежуточные итоги отображаются вверху списка элементов, а не внизу |

## Методы

| Имя | Описание |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Добавить вычисляемый элемент в сводное поле. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Получить строку формулы указанного вычисляемого поля . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Получает фильтр сводки поля сводки по типу |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Получает сводные фильтры сводного поля |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Получает, показывает ли указанное поле эти промежуточные итоги. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Устанавливает, являются ли PivotItems в сводном поле скрытыми деталями. То есть свернуть/развернуть это поле. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Устанавливает, скрыт ли конкретный PivotItem в поле данных. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Устанавливает, является ли конкретный PivotItem в сводном поле скрытым. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Инициализировать сводные элементы сводного поля |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Указывает, скрыт ли конкретный PivotItem. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Указывает, скрыт ли конкретный PivotItem. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Устанавливает, будут ли в указанном поле отображаться эти промежуточные итоги. |

### Примеры

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
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

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Изменяем атрибуты PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//делай свое дело

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Смотрите также

* пространство имен [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

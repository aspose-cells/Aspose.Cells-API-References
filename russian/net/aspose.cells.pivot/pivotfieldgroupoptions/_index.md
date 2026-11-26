---
title: "Класс PivotFieldGroupOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotFieldGroupOptions. Параметры настройки группировки полей сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Параметры настройки группировки полей сводной таблицы.

```csharp
public class PivotFieldGroupOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Получает и задает отдельные элементы группы. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Получает или задает конечное значение диапазона группировки. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Получает или задает конечное значение диапазона группировки. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Получает или задает тип группировки для поля сводной таблицы. Только для группировки поля даты и времени. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Получает или задает тип группировки для поля сводной таблицы. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Получает или задает размер интервала для каждой группы. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Получает или задает значение, указывающее, определяется ли конечное значение автоматически. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Получает или задает значение, указывающее, определяется ли начальное значение автоматически. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Получает или задает значение, указывающее, должны ли создаваться новые поля сводной таблицы после группировки. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Получает или задает начальное значение диапазона группировки. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Получает или задает начальное значение диапазона группировки. |

### Примеры

```csharp

[C#]

// Загрузить пример рабочей книги
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Получить доступ ко второму листу и его сводной таблице
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Сгруппировать первое поле строки (поле даты) по месяцам и кварталам
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Вычислите данные сводной таблицы и сохраните выходной файл
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



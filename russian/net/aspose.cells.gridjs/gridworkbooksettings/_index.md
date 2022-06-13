---
title: GridWorkbookSettings
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры рабочей книги.
type: docs
weight: 110
url: /ru/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Представляет параметры рабочей книги.

```csharp
public class GridWorkbookSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author) { get; set; } | Получает и устанавливает автора файла. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat) { get; set; } | Указывает, проверяется ли проверка пользовательского числового формата при установке Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain) { get; set; } | Указывает, создавать ли цепочку вычисляемых формул. Значение по умолчанию — ложь. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904) { get; set; } | Получает или задает значение, указывающее, используется ли в книге система дат 1904 года. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros) { get; set; } | Включить макросы; Теперь это работает только при копировании листа на другой лист в книге. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate) { get; set; } | Указывает, выполняется ли полный расчет каждый раз, когда запускается расчет. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration) { get; set; } | Указывает, использовать ли итерацию для разрешения циклических ссылок. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration) { get; set; } | Возвращает или задает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию равно 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed) { get; set; } | Истинно, если вычисления в этой книге будут выполняться только с точностью отображаемых чисел |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen) { get; set; } | Указывает, следует ли пересчитывать все формулы при открытии файла. |

### Примеры

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

 //делай свое дело

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Смотрите также

* пространство имен [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* сборка [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
---
title: "Класс GridWorkbookSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridJs.GridWorkbookSettings class. Представляет настройки рабочей книги"
type: docs
url: /ru/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Представляет настройки рабочей книги.

```csharp
public class GridWorkbookSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Получает/устанавливает автора файла. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Указывает, проверять ли пользовательский числовой формат при установке Style.Custom, по умолчанию false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, вы получите Exception. Если это свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недопустимо для формата файла Excel, не следует сохранять рабочую книгу в формате Excel позже. Иначе может возникнуть неожиданная ошибка в сгенерированном файле Excel. по умолчанию false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Указывает, создавать ли цепочку вычисляемых формул. По умолчанию false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Получает или задает значение, указывающее, использует ли рабочая книга систему дат 1904 года. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Включить макросы; Сейчас это работает только при копировании листа в другой лист в рабочей книге. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Указывает, выполнять полные вычисления каждый раз при запуске расчёта. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Указывает, использовать ли итерацию для разрешения циклических ссылок. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Возвращает или задаёт максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True, если расчёты в этой рабочей книге будут выполняться только с точностью отображаемых чисел |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Указывает, пересчитывать ли все формулы при открытии файла. По умолчанию true. |

### Примеры

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//выполняйте свою работу

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)



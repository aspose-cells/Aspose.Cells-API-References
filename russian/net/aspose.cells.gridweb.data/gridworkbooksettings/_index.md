---
title: "Класс GridWorkbookSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.GridWorkbookSettings. Представляет настройки рабочей книги."
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Представляет настройки рабочей книги.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | конструктор по умолчанию |

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Получает и задаёт автора файла. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Получает или задает, проверять ли пользовательский числовой формат при установке Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Получает или задает, создавать ли цепочку вычисляемых формул. По умолчанию false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Получает или задает значение, указывающее, использует ли рабочая книга систему дат 1904 года. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Получает или задает, включать ли макросы; сейчас это работает только при копировании листа в другой лист в рабочей книге. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Получает или задает, выполнять полные вычисления каждый раз при запуске расчёта. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Получает или задает, использовать ли итерацию для разрешения циклических ссылок. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Получает или задает максимальное количество итераций для разрешения циклической ссылки, значение по умолчанию — 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True, если расчёты в этой рабочей книге будут выполняться только с точностью отображаемых чисел |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Указывает, следует ли сохранять пробелы и переносы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Получает или задает, пересчитывать ли все формулы при открытии файла. |

### Примеры

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//выполняйте свою работу

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)



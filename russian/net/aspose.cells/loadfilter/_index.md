---
title: LoadFilter
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет фильтр предоставляющий параметры для загрузки данных при загрузке книги из шаблона.
type: docs
weight: 3980
url: /ru/net/aspose.cells/loadfilter/
---
## LoadFilter class

Представляет фильтр, предоставляющий параметры для загрузки данных при загрузке книги из шаблона.

```csharp
public class LoadFilter
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LoadFilter](loadfilter#constructor)() | Создает один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter#constructor_1)(LoadDataFilterOptions) | Создает один LoadFilter с заданными параметрами фильтра. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions) { get; set; } | Параметры фильтра для обозначения того, какие данные должны быть загружены. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder) { get; } | Указывает листы (индексы) и порядок загрузки. Значение по умолчанию равно null, что означает загрузку всех листов в порядке по умолчанию в файле шаблона. Если не null и в возвращаемом массиве нет индекса листа, то лист не будет загружен. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet)(Worksheet) | Подготавливает параметры фильтра перед загрузкой данного рабочего листа. Пользовательская реализация LoadFilter может изменить здесь LoadDataFilterOptions , чтобы указать, как загружать данные для этого рабочего листа. |

### Примечания

Пользователь может указать параметры фильтра или реализовать свой собственный LoadFilter, чтобы указать, как загружать данные.

### Примеры

В следующем примере показано, как определить параметры фильтра в соответствии со свойствами листа.

```csharp
[C#]
Workbook wb = new Workbook(template, new LoadOptions() { LoadFilter = new LoadFilterSheet() });
  //Пользовательская реализация фильтра загрузки
class LoadFilterSheet : LoadFilter
{
    public override void StartSheet(Worksheet sheet) 
    {
        if (sheet.Name == "Sheet1")
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.All;
        }
        else
        {
            LoadDataFilterOptions = Aspose.Cells.LoadDataFilterOptions.None;
        }
    }
}
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
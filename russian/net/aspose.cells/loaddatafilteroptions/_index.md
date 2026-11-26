---
title: "Перечисление LoadDataFilterOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.LoadDataFilterOptions. Представляет параметры фильтрации данных при загрузке рабочей книги из шаблона"
type: docs
url: /ru/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Представляет параметры для фильтрации данных при загрузке рабочей книги из шаблона.

```csharp
public enum LoadDataFilterOptions
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Не загружать данные листа |
| All | `2147483647` | Загрузить всё |
| CellBlank | `1` | Загрузить ячейки, значение которых пусто |
| CellString | `2` | Загрузить ячейки, значение которых является строкой |
| CellNumeric | `4` | Загрузить ячейки, значение которых числовое (включая дату и время) |
| CellError | `8` | Загрузить ячейки, значение которых является ошибкой |
| CellBool | `16` | Загрузить ячейки, значение которых является логическим |
| CellValue | `31` | Загрузить только значения ячеек (все типы значений) |
| Formula | `32` | Загрузить формулы ячеек. |
| CellData | `67108927` | Загрузить данные ячеек, включая значения, формулы и форматирование |
| Chart | `256` | Загрузить диаграммы |
| Shape | `402653696` | Загрузить фигуры |
| Drawing | `402653952` | Графические объекты (включая диаграмму, изображение, OleObject и все остальные графические объекты) |
| MergedArea | `1024` | Загрузить объединённые ячейки |
| ConditionalFormatting | `2048` | Загрузить условное форматирование |
| DataValidation | `4096` | Загрузить проверки данных |
| PivotTable | `8192` | Загрузить сводные таблицы |
| Table | `16384` | Загрузить таблицы |
| Hyperlinks | `32768` | Загрузить гиперссылки |
| SheetSettings | `65536` | Загрузить настройки листа |
| SheetData | `403701759` | Загрузить все данные листа, такие как данные ячеек, настройки, объекты и т.д. |
| BookSettings | `1048576` | Загрузить настройки книги |
| Settings | `1114112` | Загрузить настройки книги и листа |
| XmlMap | `2097152` | Загрузить XmlMap |
| Structure | `4194304` | Загрузить структуру книги |
| DocumentProperties | `8388608` | Загрузить свойства документа |
| DefinedNames | `16777216` | Загрузить определённые объекты Name |
| VBA | `33554432` | Загрузить проекты VBA |
| Style | `67108864` | Загрузить стили для форматирования ячеек |
| Picture | `134217728` | Загрузить изображения |
| OleObject | `268435456` | Загрузить OleObjects |
| Revision | `536870912` | Загрузить журналы ревизий |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Создать новый экземпляр LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Создать пользовательскую реализацию LoadFilter
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Загрузите книгу с указанными параметрами загрузки
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Сохранить книгу, чтобы проверить загруженные данные
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Пользовательская реализация LoadFilter
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Применить различные параметры фильтра в зависимости от имени листа
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



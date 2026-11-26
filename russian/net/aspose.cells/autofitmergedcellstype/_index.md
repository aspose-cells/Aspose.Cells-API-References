---
title: "Перечисление AutoFitMergedCellsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.AutoFitMergedCellsType. Представляет тип автоматического подгонения объединённых ячеек"
type: docs
url: /ru/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Представляет тип автоматической подгонки объединённых ячеек.

```csharp
public enum AutoFitMergedCellsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Игнорировать объединённые ячейки. |
| FirstLine | `1` | Только расширяет высоту первой строки. |
| LastLine | `2` | Только расширяет высоту последней строки. |
| EachLine | `3` | Расширяет высоту каждой строки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Создание экземпляра объекта Workbook
            Workbook workbook = new Workbook();
            //Получение ссылки на недавно добавленный лист
            Worksheet sheet1 = workbook.Worksheets[0];

            // Создать диапазон A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Объедините ячейки
            range.Merge();

            // Вставить значение в объединённую ячейку A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Создать объект стиля
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Включить перенос текста
            style.IsTextWrapped = true;

            // Применить стиль к ячейке
            sheet1.Cells[0, 0].SetStyle(style);

            // Создать объект для AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // Только расширяет высоту первой строки.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Автоподгонка строк на листе (включая объединённые ячейки)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Создать диапазон A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Объедините ячейки
            range2.Merge();

            // Вставить значение в объединённую ячейку A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Создать объект стиля
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Включить перенос текста
            style2.IsTextWrapped = true;

            // Применить стиль к ячейке
            sheet2.Cells[0, 0].SetStyle(style);

            // Создать объект для AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Только расширяет высоту последней строки.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Автоподгонка строк на листе (включая объединённые ячейки)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Создать диапазон A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Объедините ячейки
            range3.Merge();

            // Вставить значение в объединённую ячейку A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Создать объект стиля
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Включить перенос текста
            style3.IsTextWrapped = true;

            // Применить стиль к ячейке
            sheet3.Cells[0, 0].SetStyle(style);

            // Создать объект для AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Только расширяет высоту каждой строки.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Автоподгонка строк на листе (включая объединённые ячейки)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Создать диапазон A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Объедините ячейки
            range4.Merge();

            // Вставить значение в объединённую ячейку A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Создать объект стиля
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Включить перенос текста
            style4.IsTextWrapped = true;

            // Применить стиль к ячейке
            sheet4.Cells[0, 0].SetStyle(style);

            // Создать объект для AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Игнорировать объединённые ячейки.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Автоподгонка строк на листе (не включая объединённые ячейки)
            sheet4.AutoFitRows(options4);

            // Сохраните книгу
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



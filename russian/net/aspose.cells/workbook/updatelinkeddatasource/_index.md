---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Если эта рабочая книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников."
type: docs
url: /ru/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Если эта книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Рабочие книги, которые будут использоваться для обновления данных внешних ссылок, указанных в этой рабочей книге. Соответствие этих рабочих книг внешним ссылкам определяется по [`FileName`](../filename/) и [`DataSource`](../../externallink/datasource/). Поэтому убедитесь, что [`FileName`](../filename/) указан со правильным значением для каждой рабочей книги, чтобы они могли быть связаны с соответствующей внешней ссылкой. |

### Примечания

Если соответствующая внешняя ссылка не найдена для одной рабочей книги, эта рабочая книга будет игнорироваться. Поэтому, когда вы позже зададите формулу с новой внешней ссылкой, которую хотите связать с игнорируемой рабочей книгой, связь не будет выполнена, пока вы не вызовете этот метод снова с этими рабочими книгами.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Создайте основную рабочую книгу с внешними ссылками
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Создайте внешнюю рабочую книгу, которая будет связана
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Вызовите UpdateLinkedDataSource с массивом внешних рабочих книг
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Вычислите формулы для обновления ссылки
                mainWorkbook.CalculateFormula();

                // Отобразить обновлённое значение
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Сохранить результат
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



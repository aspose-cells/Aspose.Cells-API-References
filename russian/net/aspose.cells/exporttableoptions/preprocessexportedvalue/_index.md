---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExportTableOptions. Предобработать значение текущей ячейки для экспорта"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Предобработать значение текущей ячейки перед экспортом.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellRow | Int32 | индекс строки текущей ячейки |
| cellColumn | Int32 | индекс столбца ячейки |
| значение | CellValue | значение и тип текущей ячейки |

### Возвращаемое значение

Было ли текущая ячейка заменена другим типом и/или значением.

### Примечания

Индекс строки и столбца является абсолютным индексом ячейки в листе, а не индексом в экспортируемой таблице. Пользователь может проверить значение текущей ячейки в переопределённой реализации этого метода; если текущую ячейку необходимо заменить другим типом и значением, то в этой реализации следует установить ожидаемый тип и значение в объект CellValue и вернуть true. По умолчанию этот метод ничего не делает и возвращает false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте примерные данные в листе
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Создайте экземпляр ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Создайте объект CellValue для демонстрации
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Вызовите PreprocessExportedValue с конкретными параметрами (строка 0, столбец 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Отобразите результат вызова метода
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // При необходимости измените ячейку с обработанным значением
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Сохраните книгу
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



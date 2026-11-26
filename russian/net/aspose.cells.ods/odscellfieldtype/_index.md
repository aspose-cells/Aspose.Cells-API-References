---
title: "Перечисление OdsCellFieldType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Ods.OdsCellFieldType. Представляет тип поля ячейки ODS"
type: docs
url: /ru/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Представляет тип поля ячейки ODS.

```csharp
public enum OdsCellFieldType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Date | `0` | Текущая дата. |
| SheetName | `1` | Имя листа. |
| Title | `2` | Имя файла. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Добавить новый OdsCellField для текущей даты
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Добавить еще один OdsCellField для имени листа
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Добавить еще один OdsCellField для заголовка
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Обновить значение полей в ячейках
            odsCellFields.UpdateFieldsValue();

            // Вывести значения в консоль
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Сохраните книгу
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)



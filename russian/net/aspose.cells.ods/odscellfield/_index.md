---
title: "Класс OdsCellField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Ods.OdsCellField. Представляет ячейковое поле ODS."
type: docs
url: /ru/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Представляет ячейку поля ODS.

```csharp
public class OdsCellField
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Получает и задает индекс столбца ячейки. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Представляет пользовательский формат значения поля. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Получает и задает тип поля. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Получает и задает индекс строки ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Создайте OdsCellField через коллекцию (без конструктора без параметров)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Получите поле, которое мы только что добавили
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Запишите что‑нибудь в ячейку, идентифицированную OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Добавьте то же поле ещё раз, чтобы продемонстрировать использование коллекции (необязательно)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Обновите все поля ODS, чтобы они отразились в сохранённом файле
                odsFields.UpdateFieldsValue();

                // Отобразите значения свойств в консоли
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Сохраните книгу в виде файла ODS
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)



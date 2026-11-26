---
title: "OdsCellFieldCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsCellFieldCollection. Получает поле по индексу"
type: docs
url: /ru/net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

Получает поле по индексу.

```csharp
public OdsCellField this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить ячейки ODS с параметром формата
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
            sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");

            // Получить доступ к полям с помощью свойства Item
            OdsCellField titleField = sheet.Cells.OdsCellFields[0];
            OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];

            // Вывести типы полей
            Console.WriteLine("Field 0 Type: " + titleField.FieldType);
            Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);

            // Сохранить и загрузить
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Проверить сохранённые поля
            Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### См. также

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

Получает поле по индексу строки и столбца.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки. |
| column | Индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить несколько ячеек ODS
            // (строка, столбец, тип поля, формат)
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "TitleFormat");
            sheet.Cells.OdsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);

            try
            {
                // Получайте доступ к полям, используя свойство Item (индексатор)
                // 1) По индексу коллекции
                OdsCellField firstField = sheet.Cells.OdsCellFields[0];
                Console.WriteLine("First field type (by index): " + firstField.FieldType);

                // 2) По позиции ячейки (строка, столбец)
                OdsCellField titleField = sheet.Cells.OdsCellFields[0, 0];
                Console.WriteLine("Field at (0,0) type (by position): " + titleField.FieldType);

                // Обновите ячейки значениями полей
                sheet.Cells.OdsCellFields.UpdateFieldsValue();

                // Сохраните книгу (формат ODS сохраняет поля)
                workbook.Save("OdsCellFieldItemDemo.ods");
                Console.WriteLine("Workbook saved as OdsCellFieldItemDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



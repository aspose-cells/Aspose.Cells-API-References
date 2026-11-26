---
title: "Cells.OdsCellFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает список полей ods"
type: docs
url: /ru/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Получает список полей ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию Cells
            Cells cells = worksheet.Cells;

            try
            {
                // Получить доступ к свойству OdsCellFields (только для чтения)
                var odsCellFields = cells.OdsCellFields;

                // Отобразить информацию о коллекции OdsCellFields
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Итерировать коллекцию OdsCellFields
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Продемонстрировать обновление значений полей
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



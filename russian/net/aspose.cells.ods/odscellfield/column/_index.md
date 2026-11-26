---
title: "OdsCellField.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsCellField. Получает и задает индекс столбца ячейки"
type: docs
url: /ru/net/aspose.cells.ods/odscellfield/column/
---
## OdsCellField.Column property

Получает и задает индекс столбца ячейки.

```csharp
public int Column { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Добавьте поля с разными типами и продемонстрируйте свойство Column
            odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);

            // Доступ и отображение свойства Column
            Console.WriteLine("Field Columns:");
            foreach (OdsCellField field in odsCellFields)
            {
                Console.WriteLine($"Type: {field.FieldType}, Column: {field.Column}");
                worksheet.Cells[field.Row, field.Column].PutValue($"Column: {field.Column}");
            }

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldColumnDemo.ods");
        }
    }
}
```

### См. также

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



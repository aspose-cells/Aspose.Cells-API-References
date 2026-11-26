---
title: "OdsCellField.FieldType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsCellField. Получает и задает тип поля"
type: docs
url: /ru/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Получает и задает тип поля.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyFieldTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить ячейки ODS с разными типами полей и строками формата
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // Продемонстрировать использование свойства FieldType
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Проверить FieldType после перезагрузки
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### См. также

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



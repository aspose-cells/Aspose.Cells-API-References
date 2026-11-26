---
title: "OdsCellFieldCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод OdsCellFieldCollection. Добавляет поле"
type: docs
url: /ru/net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

Добавляет поле.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |
| fieldType | OdsCellFieldType | Тип поля. |
| формат | String | Числовой формат поля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionMethodAddWithInt32Int32OdsCellFieldTypStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Добавить разные типы полей
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldsDemo.ods");
        }
    }
}
```

### См. также

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



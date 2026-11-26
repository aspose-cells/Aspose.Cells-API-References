---
title: "OdsCellField.CustomFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsCellField. Представляет пользовательский формат значения поля"
type: docs
url: /ru/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Представляет пользовательский формат значения поля.

```csharp
public string CustomFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyCustomFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Поле даты с пользовательским форматом
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Поле имени листа без пользовательского формата
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Поле заголовка с пользовательским форматом (демонстрирует строковый формат)
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, "Title Format: @");
            
            odsCellFields.UpdateFieldsValue();
            
            foreach (OdsCellField field in odsCellFields)
            {
                worksheet.Cells[field.Row, field.Column].PutValue(
                    $"Type: {field.FieldType}, Format: {field.CustomFormat ?? "None"}");
            }
            
            workbook.Save("OdsCellFieldCustomFormatDemo.ods");
        }
    }
}
```

### См. также

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



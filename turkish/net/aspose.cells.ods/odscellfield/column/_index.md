---
title: "OdsCellField.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsCellField özelliği. Hücrenin sütun indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.ods/odscellfield/column/
---
## OdsCellField.Column property

Hücrenin sütun indeksini alır ve ayarlar.

```csharp
public int Column { get; set; }
```

### Örnekler

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

            // Farklı tiplerde alanlar ekle ve Column özelliğini göster
            odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);

            // Column özelliğine eriş ve görüntüle
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

### Ayrıca Bakınız

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



---
title: "OdsCellField.CustomFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsCellField özelliği. Alanın değerinin özel biçimini temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Alan değerinin özel biçimini temsil eder.

```csharp
public string CustomFormat { get; set; }
```

### Örnekler

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
            
            // Özel biçimli tarih alanı
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Özel biçim olmadan sayfa adı alanı
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Özel biçimli başlık alanı (dize biçimini göstererek)
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

### Ayrıca Bakınız

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



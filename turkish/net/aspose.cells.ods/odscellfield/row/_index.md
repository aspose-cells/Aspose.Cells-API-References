---
title: "OdsCellField.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsCellField özelliği. Hücrenin satır indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.ods/odscellfield/row/
---
## OdsCellField.Row property

Hücrenin satır indeksini alır ve ayarlar.

```csharp
public int Row { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Farklı tiplerde alanlar ekle
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
            
            odsCellFields.UpdateFieldsValue();

            // Row özelliğinin kullanımını göster
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                int row = field.Row; // Using Row property
                worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
            }

            workbook.Save("OdsCellFieldRowDemo.ods");
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



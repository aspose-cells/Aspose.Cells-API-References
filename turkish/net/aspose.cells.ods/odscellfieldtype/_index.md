---
title: "Enum OdsCellFieldType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. ods hücre alanı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

ods'nin hücre alanı türünü temsil eder.

```csharp
public enum OdsCellFieldType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Date | `0` | Geçerli tarih. |
| SheetName | `1` | Sayfanın adı. |
| Title | `2` | Dosyanın adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir OdsCellFieldCollection oluştur
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Geçerli tarih için yeni bir OdsCellField ekle
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Sayfa adı için bir başka OdsCellField ekle
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Başlık için bir başka OdsCellField ekle
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Alanların değerini hücrelere güncelle
            odsCellFields.UpdateFieldsValue();

            // Değerleri konsola çıktı olarak ver
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)



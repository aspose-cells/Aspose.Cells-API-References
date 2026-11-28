---
title: "OdsCellField.FieldType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsCellField özelliği. Alanın tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Alan tipini alır ve ayarlar.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Farklı alan tipleri ve format dizgeleriyle ODS hücre alanları ekle
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // FieldType özelliği kullanımını göster
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Kalıcılığı göstermek için kaydedin ve yeniden yükleyin
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Yeniden yüklemeden sonra FieldType'ı doğrula
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)



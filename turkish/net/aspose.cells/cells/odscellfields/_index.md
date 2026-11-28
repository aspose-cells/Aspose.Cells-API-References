---
title: "Cells.OdsCellFields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. ODS'nin alan listesini alır"
type: docs
url: /tr/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

ods'nin alan listesini alır.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Cells koleksiyonunu al
            Cells cells = worksheet.Cells;

            try
            {
                // OdsCellFields özelliğine eriş (yalnızca okunur)
                var odsCellFields = cells.OdsCellFields;

                // OdsCellFields koleksiyonu hakkında bilgi göster
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // OdsCellFields koleksiyonunda yinele
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Alan değerlerini güncellemeyi göster
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

### Ayrıca Bakınız

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



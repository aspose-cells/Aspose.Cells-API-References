---
title: "Workbook.GetDigitalSignature"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Dosyadan dijital imzayı alır"
type: docs
url: /tr/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Dosyadan dijital imzayı alır.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Dijital imzaları almak için GetDigitalSignature yöntemini çağır
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Dijital imzalar hakkında bilgileri göster
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Protection.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection yöntemi. Koruma bilgilerini kopyala."
type: docs
url: /tr/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Koruma bilgilerini kopyala.

```csharp
public void Copy(Protection source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Protection |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kaynak koruma ayarlarını oluşturun - çalışma sayfasından mevcut korumayı kullanın.
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Hedef koruma ayarlarını al
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Protection parametresiyle Copy metodunu çağır
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



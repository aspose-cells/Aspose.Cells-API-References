---
title: "Workbook.RemoveExternalLinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Çalışma kitabındaki tüm dış bağlantıları kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Çalışma kitabındaki tüm dış bağlantıları kaldırır.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalLinkCollection.Clear() yöntemini kullanın. Bu yöntem, Aralık 2021'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
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
                // RemoveExternalLinks yöntemini çağırın
                workbook.RemoveExternalLinks();

                // Yöntem çağrısının sonuçlarını veya etkilerini göster
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Değişiklik yapıldıysa çalışma kitabını kaydet
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



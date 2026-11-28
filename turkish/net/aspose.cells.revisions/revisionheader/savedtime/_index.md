---
title: "RevisionHeader.SavedTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionHeader özelliği. Bu revizyon setinin kaydedildiği tarih ve saati alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Bu revizyon seti kaydedildiğinde tarih ve saati alır ve ayarlar

```csharp
public DateTime SavedTime { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir revision header örneği oluştur
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // SavedTime özelliğini ayarla
                revisionHeader.SavedTime = DateTime.Now;
                
                // SavedTime değerini al ve göster
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // SavedTime özelliğini değiştir
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Özelliğin kullanıldığını göstermek için çalışma kitabını kaydet
                workbook.Save("SavedTimeDemo.xlsx");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



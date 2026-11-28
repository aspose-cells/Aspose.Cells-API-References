---
title: "RevisionHeader.UserName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionHeader özelliği. Revizyon yapan kullanıcının adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Revizyonu yapan kullanıcının adını alır ve ayarlar

```csharp
public string UserName { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Bir RevisionHeader örneği oluştur
                RevisionHeader revisionHeader = new RevisionHeader();

                // UserName özelliğini ayarla
                revisionHeader.UserName = "JohnDoe";

                // UserName özelliğinin mevcut değerini göster
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // UserName özelliğini değiştir
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Özelliğin kullanıldığını göstermek için çalışma kitabını kaydet
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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



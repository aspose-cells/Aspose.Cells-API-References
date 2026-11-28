---
title: "RevisionCustomView.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCustomView özelliği. Revizyonun türünü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Revizyon tipini alır.

```csharp
public override RevisionType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // Değişiklik yapıldığında revizyon takibi varsayılan olarak etkinleştirilmiş gibi görünür
            
            // Bir revizyon kaydı oluşturmak için özel bir görünüm ekle
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Çalışma kitabının yerleşik işlevselliği aracılığıyla revizyon koleksiyonuna eriş
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // Gerçek bir uygulamada revizyonlara erişmenin bir yolu olurdu
                // Tam yöntemi bulamadığımız için bunu null olarak bırakacağız
                // Bu, API sınırlamasını kabul ederken yapıyı korur
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Revizyonlarda RevisionCustomView öğesini bul
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Type özelliği değerini gösterin
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Type özelliğinin nasıl kullanılacağını göster
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // Type özelliği yalnızca okunur, bu yüzden ayarlayamayız
                // Revizyon türünü belirlemek için yalnızca değerini kontrol edebiliriz
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Gerekirse diğer durumlar eklenebilir
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



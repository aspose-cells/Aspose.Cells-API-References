---
title: "ExternalLinkCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLinkCollection metodu. Harici bir bağlantı ekler"
type: docs
url: /tr/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Bir dış bağlantı ekler.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Harici dosya adı. |
| sheetNames | String[] | Dış dosyanın tüm sayfa adları. |

### Dönüş Değeri

Bu listedeki dış adın konumu.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Dış bağlantılar koleksiyonunu al
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Add yöntemi için parametreleri hazırlayın
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Add yöntemini (String, String[]) parametreleriyle çağırın
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Eklenen dış bağlantı bilgilerini göster
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link file: {link.DataSource}");
                Console.WriteLine("Referenced sheets:");
                foreach (string sheet in sheetNames)
                {
                    Console.WriteLine($"- {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Bir dış bağlantı ekle .

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directoryType | DirectoryType | Dosya adının dizin türü. |
| fileName | String | dosya adı. |
| sheetNames | String[] | Dış dosyanın tüm sayfa adları. |

### Dönüş Değeri

Bu listedeki dış adın konumu.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Dış bağlantılar koleksiyonunu al
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Add yöntemi için parametreleri hazırlayın
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Add yöntemini (DirectoryType, String, String[]) parametreleriyle çağırın
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Eklenen dış bağlantı hakkında bilgileri göster
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link references: {link.DataSource}");
                foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
                {
                    Console.WriteLine($" - References sheet: {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



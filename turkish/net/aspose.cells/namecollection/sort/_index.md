---
title: "NameCollection.Sort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Tanımlı adları sıralar"
type: docs
url: /tr/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Tanımlı isimleri sıralar.

```csharp
public void Sort()
```

### Açıklamalar

Excel dosyasında çok sayıda adlandırılmış aralık oluşturursanız, lütfen bu yöntemi tüm adlandırılmış aralıklar oluşturulduktan ve kaydetmeden önce çağırın

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma kitabından NameCollection'ı alın
            NameCollection names = workbook.Worksheets.Names;
            
            // Sıralamayı göstermek için bazı adlandırılmış aralıklar ekleyin
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Sıralamadan önce adları göster
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Sort yöntemini çağırın
                names.Sort();
                
                // Sıralamadan sonra adları göster
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



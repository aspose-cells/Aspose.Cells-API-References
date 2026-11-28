---
title: "NameCollection.Remove"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Bir dizi adı kaldır"
type: docs
url: /tr/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

İsim dizisini kaldır.

```csharp
public void Remove(string[] names)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adlar | String[] | Adların metni. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma kitabından NameCollection'ı alın
            NameCollection names = workbook.Worksheets.Names;
            
            // Kaldırmayı göstermek için bazı adlandırılmış aralıklar ekle
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Kaldırılacak adların dizisini hazırla
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // String[] parametresiyle Remove yöntemini çağır
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Kalan adları göster
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

İsmi kaldır.

```csharp
public void Remove(string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Adın metni. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Bir adlandırılmış aralık ekle
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Kaldırmadan önce sayıyı göster
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Adlandırılmış aralığı kaldır
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Kaldırmadan sonra sayıyı göster
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



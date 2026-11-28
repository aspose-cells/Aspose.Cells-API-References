---
title: "NameCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection özelliği. Belirtilen indeksteki Name öğesini alır"
type: docs
url: /tr/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Belirtilen indeksteki [`Name`](../../name/) öğesini alır.

```csharp
public Name this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // İsim koleksiyonuna eriş.
            NameCollection names = workbook.Worksheets.Names;
            
            // Doğru metod imzasını kullanarak adlandırılmış aralıklar ekle
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Item özelliğinin kullanımını göster
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Item özelliğini kullanarak ada göre eriş
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Adlandırılmış bir aralığı değiştir
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Belirtilen adla [`Name`](../../name/) öğesini alır.

```csharp
public Name this[string text] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| metin | Ad metni. |

### Dönüş Değeri

Belirtilen ada sahip öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfalarının ad koleksiyonuna eriş
            NameCollection names = workbook.Worksheets.Names;
            
            // Bazı adlandırılmış aralıklar ekle (doğru Add metod imzasını kullanacak şekilde düzeltildi)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Item özelliğini kullanarak adlandırılmış aralıklara eriş
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Adların mevcut olduğunu doğrula
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Var olmayan bir ada erişmeye çalış
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



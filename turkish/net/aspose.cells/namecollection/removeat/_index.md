---
title: "NameCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Belirli indeksteki adı kaldırır"
type: docs
url: /tr/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Belirli indeksteki adı kaldır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | kaldırılacak Name'in indeksi. |

### Açıklamalar

Lütfen yöntemi çağırmadan önce adın diğer formüller tarafından referans alınmadığından emin olun. Ve eğer ad referans alınıyorsa, Name.RefersTo'yi null olarak ayarlamak daha iyidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Koleksiyona adlar ekle
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // İndexe göre adı kaldır
            names.RemoveAt(firstIndex);

            // Kaldırmayı sayıyı kontrol ederek doğrula
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



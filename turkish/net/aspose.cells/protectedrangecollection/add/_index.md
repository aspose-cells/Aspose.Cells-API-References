---
title: "ProtectedRangeCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRangeCollection yöntemi. Koleksiyona bir ProtectedRange öğesi ekler"
type: docs
url: /tr/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Koleksiyona bir [`ProtectedRange`](../../protectedrange/) öğesi ekler.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Aralık başlığı. Bu, bir tanımlayıcı olarak kullanılır, adlandırılmış aralık tanımı olarak değil. |
| startRow | Int32 | Aralığın başlangıç satır indeksi. |
| startColumn | Int32 | Aralığın başlangıç sütun indeksi. |
| endRow | Int32 | Aralığın bitiş satır indeksi. |
| endColumn | Int32 | Aralığın bitiş sütun indeksi. |

### Dönüş Değeri

nesne indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Adı ve koordinatlarıyla korumalı bir aralık ekleyin
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Eklenen aralığa erişin
            ProtectedRange range = pranges[index];
            
            // Güvenlik tanımlayıcısını ayarla
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Kaydet ve doğrula
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



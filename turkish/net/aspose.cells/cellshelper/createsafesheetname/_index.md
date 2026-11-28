---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa onu döndürür. Aksi takdirde, uzunluk sınırı aşılırsa dize kesilir ve geçersiz karakterler   ile değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür."
type: docs
url: /tr/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluğu limiti aşarsa dize kesilir ve geçersiz karakterler ' ' ile değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| nameProposal | String | kullanılacak sayfa adı |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluğu limiti aşarsa dize kesilir ve geçersiz karakterler verilen karakterle değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| nameProposal | String | kullanılacak sayfa adı |
| replaceChar | Char | verilen sayfa adındaki geçersiz karakterleri değiştirmek için kullanılacak karakter |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Örnek 1: Varsayılan değiştirme karakteri ile güvenli sayfa adı oluştur
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Örnek 2: Özel değiştirme karakteri 'A' ile güvenli sayfa adı oluştur
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



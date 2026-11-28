---
title: "Worksheet.Protect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Çalışma sayfasını korur"
type: docs
url: /tr/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Çalışma sayfasını korur.

```csharp
public void Protect(ProtectionType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ProtectionType | Koruma türü. |

### Açıklamalar

Bu yöntem, çalışma sayfasını şifre olmadan korur. Çalışma sayfasını Excel dosyasının tüm sürümlerinde koruyabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını Nesneler koruma türüyle koruyun
            sheet.Protect(ProtectionType.Objects);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Çalışma sayfasını korur.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ProtectionType | Koruma türü. |
| parola | String | Şifre. |
| oldPassword | String | Çalışma sayfası zaten bir şifreyle korunuyorsa, lütfen eski şifreyi sağlayın. Aksi takdirde, bu parametreye null değer veya boş dize ayarlayabilirsiniz. |

### Açıklamalar

Bu yöntem, Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını şifre ile koruyun ve tüm koruma türlerine izin verin
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



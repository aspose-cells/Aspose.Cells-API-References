---
title: "ExternalLinkCollection.Clear"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLinkCollection yöntemi. Tüm dış bağlantıları kaldırır"
type: docs
url: /tr/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Tüm dış bağlantıları kaldırır.

```csharp
public void Clear()
```

### Açıklamalar

Dış bağlantılar kaldırıldığında, onlara başvuran tüm formüller de geçersiz referanslar haline geldiği için kaldırılacaktır.

### Ayrıca Bakınız

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Tüm dış bağlantıları kaldırır.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Formüllerdeki dış bağlantı referanslarının tümünü mevcut çalışma kitabının referanslarına güncelleyip güncellemeyeceği. |

### Açıklamalar

Eğer referansların güncellenmesi gerekiyorsa, formüllerdeki dış bağlantı referansları mümkün olduğunda mevcut çalışma kitabına değiştirilecektir. Örneğin, bir hücrenin orijinal formülü \"='externalsource.xlam'!customfunction()\" iken, dış bağlantılar kaldırıldıktan sonra formül \"=customfunction()\" olur; Orijinal formül \"='[externalsource.xlam]Sheet1'!$A$1\" olduğunda, mevcut çalışma kitabında \"Sheet1\" adlı bir sayfa olup olmadığına göre: doğru ise formül \"=Sheet1!$A$1\" olur; yanlış ise formül \"=#REF!$A$1\" olur. Referansların güncellenmesi gerekmiyorsa, dış bağlantılara başvuran tüm formüller de geçersiz referanslar haline geldiği için kaldırılacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı dış bağlantılar ekle
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // updateReferences = true ile temizle
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Bağlantıları tekrar ekle
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // updateReferences = false ile temizle
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



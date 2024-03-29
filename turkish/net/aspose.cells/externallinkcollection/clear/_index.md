---
title: Clear
second_title: Aspose.Cells for .NET API Referansı
description: Tüm harici bağlantıları kaldırır.
type: docs
weight: 40
url: /tr/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Tüm harici bağlantıları kaldırır.

```csharp
public void Clear()
```

### Notlar

Harici bağlantıları kaldırırken, bunlara referans veren tüm formüller de kaldırılacaktır çünkü referanslar geçersiz hale gelir.

### Ayrıca bakınız

* class [ExternalLinkCollection](../../externallinkcollection)
* ad alanı [Aspose.Cells](../../externallinkcollection)
* toplantı [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Tüm harici bağlantıları kaldırır.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Harici bağlantıların tüm referanslarını mevcut çalışma kitabının referansları olarak güncelleyip güncellemeyeceği. |

### Notlar

Referansların güncellenmesi gerekiyorsa, formüllerdeki harici bağlantılara yapılan referanslar mevcut çalışma kitabına değiştirilir. Örneğin, bir hücrenin orijinal formülü "='externalsource.xlam'!customfunction()", harici bağlantılar kaldırıldıktan sonra, formül "=özel işlev()" olur. Referansların güncellenmesi gerekmiyorsa, harici linkler referanslarına sahip tüm formüller de bu referanslar geçersiz olacağından kaldırılacaktır.

### Ayrıca bakınız

* class [ExternalLinkCollection](../../externallinkcollection)
* ad alanı [Aspose.Cells](../../externallinkcollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

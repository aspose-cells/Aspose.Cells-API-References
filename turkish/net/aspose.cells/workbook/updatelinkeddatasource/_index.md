---
title: UpdateLinkedDataSource
second_title: Aspose.Cells for .NET API Referansı
description: Bu çalışma kitabı başka bir veri kaynağına harici bağlantılar içeriyorsa Aspose.Cells en son verileri almaya çalışır.
type: docs
weight: 660
url: /tr/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Bu çalışma kitabı başka bir veri kaynağına harici bağlantılar içeriyorsa, Aspose.Cells en son verileri almaya çalışır.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Harici çalışma kitaplarına bu çalışma kitabı referans verir. Null ise doğrudan harici bağlantılı dosyaları açacağız.. Null değilse, önce dizideki harici linkin olup olmadığını kontrol edeceğiz; değilse, açacağız harici bağlantılı dosyalar yeniden. |

### Notlar

Formüller hesaplanmadan önce yöntem çağrılmazsa, Aspose.Cells önceki bilgileri kullanır (dosyada önbelleğe alınır); Lütfen CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath'i ayarlayın. Ve lütfen bu çalışma kitabı bir akıştan geliyorsa Workbook.FilePath'i ayarlayın, aksi takdirde Aspose.Cells bazen harici bağlantının tam yolunu alamaz.

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

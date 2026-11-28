---
title: "Worksheet.FilterString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet method. Sütun için filtreyi ayarlar. filterString'i çağırmadan önce AddAutoFilter'i çağırmamız gerektiğine dikkat edin. Filtre kriteri dizesi. Virgülü ayırıcı karakter olarak kullandığımıza dikkat edin, bu yüzden filtrelemek istediğiniz hücre değeri virgül içermemelidir. filterString10123456, 10. sütunun 123 veya 456 içermesi anlamına gelir. filterString10123, 10. sütunun 123 içermesi anlamına gelir, değer virgülle ayrılmıştır. örn. 123456789 veya abc"
type: docs
url: /tr/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

Sütun için filtreyi ayarlar. filterString'i çağırmadan önce AddAutoFilter'i çağırmanız gerekir. Filtre kriteri dizesi. Virgül-&gt;"," karakterini ayırıcı olarak kullandığımızı unutmayın, bu yüzden filtrelemek istediğiniz hücre değeri virgül içermemelidir. filterString(10,"123,456") ifadesi, 10. sütunun 123 veya 456 içermesi anlamına gelir, filterString(10,"123") ifadesi, 10. sütunun 123 içermesi anlamına gelir; değer virgülle ayrılmış olmalıdır, örn. 123,456,789 veya abc

```csharp
public void FilterString(int column, string criteria)
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)



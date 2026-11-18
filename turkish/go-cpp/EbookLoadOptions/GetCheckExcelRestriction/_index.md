---
title: "GetCheckExcelRestriction Metodu"
linktitle: "GetCheckExcelRestriction"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "GetCheckExcelRestriction yöntemi. Go'da getcheckexcelrestriction işlevini temsil eden fonksiyonu kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/ebookloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir.

```go

func (instance *EbookLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## Açıklamalar


## Ayrıca Bakınız

* Class [EbookLoadOptions](../)
* Library [Aspose.Cells for Go](../../)

---
title: "CalculationData Sınıfı"
linktitle: "CalculationData"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CalculationData sınıfı. Go'da calculationdata nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/calculationdata/
---

## CalculationData class

Bir işlev hesaplanırken, işlev adı, parametreler vb. gibi gerekli verileri temsil eder.

```go

type CalculationData struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetCalculatedValue](./getcalculatedvalue/) | Bu işlev için hesaplanmış değeri alır veya ayarlar. |
| [SetCalculatedValue](./setcalculatedvalue/) | Bu işlev için hesaplanmış değeri alır veya ayarlar. |
| [GetWorkbook](./getworkbook/) | İşlevin bulunduğu Workbook nesnesini alır. |
| [GetWorksheet](./getworksheet/) | İşlevin bulunduğu Worksheet nesnesini alır. |
| [GetCellRow](./getcellrow/) | İşlevin bulunduğu hücrenin satır indeksini alır. |
| [GetCellColumn](./getcellcolumn/) | İşlevin bulunduğu hücrenin sütun indeksini alır. |
| [GetCell](./getcell/) | İşlevin bulunduğu Cell nesnesini alır. |
| [GetFunctionName](./getfunctionname/) | Hesaplanacak işlev adını alır. |
| [GetParamCount](./getparamcount/) | Parametre sayısını alır |
| [GetParamValue](./getparamvalue/) | Belirli bir dizindeki parametrenin temsil edilen değer nesnesini alır. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Belirli bir dizindeki parametrenin değer(ler)ini alır.Eğer parametre hesaplanması gereken bir ifade ise, dizi modunda hesaplanacaktır. |
| [GetParamText](./getparamtext/) | Verilen dizindeki parametrenin literal metnini alır. |

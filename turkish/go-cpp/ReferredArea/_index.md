---
title: "ReferredArea Sınıfı"
linktitle: "ReferredArea"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ReferredArea sınıfı. Go'da referredarea'yı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/referredarea/
---

## ReferredArea class

Formül tarafından başvurulan bir alanı temsil eder.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | Bunun harici bir bağlantı olup olmadığını gösterir. |
| [GetExternalFileName](./getexternalfilename/) | Bu harici bir referans ise harici dosya adını al. |
| [GetSheetName](./getsheetname/) | Bu referansın hangi sayfada olduğunu gösterir. |
| [GetSheetNames](./getsheetnames/) | Bu örneğin referans verdiği tüm çalışma sayfalarının adları. |
| [IsEntireRow](./isentirerow/) | Bu alanın tüm sütunları (tam satır) içerip içermediğini gösterir. |
| [IsEntireColumn](./isentirecolumn/) | Bu alanın tüm satırları (tam sütun) içerip içermediğini gösterir. |
| [IsArea](./isarea/) | Bunun bir alan olup olmadığını gösterir. |
| [GetEndColumn](./getendcolumn/) | Alanının son sütunu. |
| [GetStartColumn](./getstartcolumn/) | Alanının başlangıç sütunu. |
| [GetEndRow](./getendrow/) | Alanının son satırı. |
| [GetStartRow](./getstartrow/) | Alanının başlangıç satırı. |
| [GetValues](./getvalues/) | Bu alandaki hücre değerlerini alır. |
| [GetValues_Bool](./getvalues_bool/) | Bu alandaki hücre değerlerini alır. |
| [GetValue_Int_Int](./getvalue_int_int/) | Bu alanın sol üst köşesinden verilen ofsetle hücre değerini alır. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Bu alanın sol üst köşesinden verilen ofsetle hücre değerini alır. |
| [ToString](./tostring/) | Bu alanın referans adresini döndürür.Genellikle formülde kullanılabilecek referansın adresidir, örneğin "Sheet1!A1:C3". |

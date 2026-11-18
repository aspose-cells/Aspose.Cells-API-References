---
title: "IconSet Sınıfı"
linktitle: "IconSet"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "IconSet sınıfı. Go dilinde iconset'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/iconset/
---

## IconSet class

IconSet koşullu biçimlendirme kuralını açıklar. Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular.

```go

type IconSet struct  {
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
| [GetCfIcons](./getcficons/) | Koleksiyondan theConditionalFormattingIcon'i al. |
| [GetCfvos](./getcfvos/) | CFValueObjects örneğini alın. |
| [GetType](./gettype/) | Görüntülemek için simge seti türünü Alın veya Ayarlayın. Tür ayarlandığında, mevcut Cfvos'un sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuz ise, eski Cfvos temizlenir ve varsayılan Cfvos eklenir. |
| [SetType](./settype/) | Görüntülemek için simge seti türünü Alın veya Ayarlayın. Tür ayarlandığında, mevcut Cfvos'un sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuz ise, eski Cfvos temizlenir ve varsayılan Cfvos eklenir. |
| [IsCustom](./iscustom/) | Simge setinin özelleştirilmiş olup olmadığını gösterir. Varsayılan değer false. |
| [GetShowValue](./getshowvalue/) | Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer true. |
| [SetShowValue](./setshowvalue/) | Bu simge setinin uygulandığı hücrelerin değerlerini gösterip göstermeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer true. |
| [GetReverse](./getreverse/) | Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer false. |
| [SetReverse](./setreverse/) | Bu simge setindeki simgelerin varsayılan sırasını tersine çevirip çevirmeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer false. |

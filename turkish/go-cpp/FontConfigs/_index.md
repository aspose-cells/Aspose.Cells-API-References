---
title: "FontConfigs Sınıfı"
linktitle: "FontConfigs"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FontConfigs sınıfı. Go'da fontconfigs'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/fontconfigs/
---

## FontConfigs class

Yazı tipi ayarlarını belirtir

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Yazı tipinin mevcut olup olmadığını belirtin. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Yazı tipi dosyası verisinin veri bilgilerini alın. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Varsayılan yazı tipi adını alır veya ayarlar. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Varsayılan yazı tipi adını alır veya ayarlar. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Bir yazı tipi mevcut olmadığında ve bu yazı tipinin ikamesi ayarlanmamış olduğunda, sistem yazı tipi ikamelerini önce kullanıp kullanmayacağını belirtin. Örneğin Ubuntu'da "Arial" yazı tipi genellikle "Liberation Sans" ile ikame edilir. Varsayılan değer false'tur. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Bir yazı tipi mevcut olmadığında ve bu yazı tipinin ikamesi ayarlanmamış olduğunda, sistem yazı tipi ikamelerini önce kullanıp kullanmayacağını belirtin. Örneğin Ubuntu'da "Arial" yazı tipi genellikle "Liberation Sans" ile ikame edilir. Varsayılan değer false'tur. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Verilen orijinal yazı tipi adı için yazı tipi ikame adları. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi döndürür. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Font klasörünü ayarlar |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Font klasörünü ayarlar |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Font kaynaklarını ayarlar. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Kaynakların listesini içeren dizinin bir kopyasını alır |

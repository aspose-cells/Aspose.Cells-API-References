---
title: "AbstractLowCodeSaveOptionsProvider Sınıfı"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AbstractLowCodeSaveOptionsProvider sınıfı. Go dilinde abstractlowcodesaveoptionsprovider nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Birden fazla çıktı gerektiren süreçler için birden fazla kaydetme seçeneği sağlamak amacıyla uygulama. Örneğin, <see cref="SpreadsheetSplitter"/> özelliği bölünmüş dosyaları kaydetmek için birden fazla hedef gerektirir.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
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
| [GetSaveOptions](./getsaveoptions/) | Mevcut bölünmüş parçanın çıktı ayarlarını almak için kullanılan kaydetme seçeneklerini alır. Null döndürmek, verilen parçayı atlamak anlamına gelir. |
| [Finish](./finish/) | Mevcut bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. |

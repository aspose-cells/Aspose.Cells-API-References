---
title: "LowCodeSaveOptions Sınıfı"
linktitle: "LowCodeSaveOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LowCodeSaveOptions sınıfı. Go'da lowcodesaveoptions nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Oluşturulan sonuçları düşük kod yöntemiyle kaydetme seçenekleri.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetOutputFile](./getoutputfile/) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş string dışındaki bir değerle ayarladığınızda OutputStream yoksayılacaktır. |
| [SetOutputFile](./setoutputfile/) | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş string dışındaki bir değerle ayarladığınızda OutputStream yoksayılacaktır. |
| [GetOutputStream](./getoutputstream/) | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda OutputFile yoksayılacaktır. |
| [SetOutputStream](./setoutputstream/) | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda OutputFile yoksayılacaktır. |
| [GetSaveFormat](./getsaveformat/) | Çıktı için kaydetme biçimini alır ve ayarlar.Genel olarak, düşük kodlu yöntemle belirli bir işlem için yalnızca bazı belirli biçimlere izin verilir.Lütfen ilgili işlem için doğru biçimi belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir. |
| [SetSaveFormat](./setsaveformat/) | Çıktı için kaydetme biçimini alır ve ayarlar.Genel olarak, düşük kodlu yöntemle belirli bir işlem için yalnızca bazı belirli biçimlere izin verilir.Lütfen ilgili işlem için doğru biçimi belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir. |

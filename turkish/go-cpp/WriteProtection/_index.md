---
title: "WriteProtection Sınıfı"
linktitle: "WriteProtection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "WriteProtection sınıfı. Go'da writeprotection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/writeprotection/
---

## WriteProtection class

Bir çalışma kitabı için yazma koruma ayarlarını belirtir.

```go

type WriteProtection struct  {
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
| [GetAuthor](./getauthor/) | Yazarı alır ve ayarlar. |
| [SetAuthor](./setauthor/) | Yazarı alır ve ayarlar. |
| [GetRecommendReadOnly](./getrecommendreadonly/) | Read Only Recommended seçeneğinin seçili olup olmadığını gösterir. |
| [SetRecommendReadOnly](./setrecommendreadonly/) | Read Only Recommended seçeneğinin seçili olup olmadığını gösterir. |
| [IsWriteProtected](./iswriteprotected/) | Bu çalışma kitabının yazma korumalı olup olmadığını gösterir. |
| [GetPassword](./getpassword/) | Dosyayı değiştirmek için korumalı şifreyi ayarlar. |
| [SetPassword](./setpassword/) | Dosyayı değiştirmek için korumalı şifreyi ayarlar. |
| [ValidatePassword](./validatepassword/) | Belirtilen şifre, dosyanın korumalı olduğu yazma koruma şifresiyle aynıysa doğru döndürür. |

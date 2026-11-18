---
title: "FileFormatInfo Sınıfı"
linktitle: "FileFormatInfo"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FileFormatInfo sınıfı. Go dilinde fileformatinfo nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/fileformatinfo/
---

## FileFormatInfo class

<see cref=\"FileFormatUtil\"/> dosya formatı tespit yöntemleri tarafından döndürülen verileri içerir.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Dosyanın Microsoft Rights Management Server tarafından korunup korunmadığını gösterir. |
| [IsEncrypted](./isencrypted/) | Belge şifrelenmiş ve açmak için parola gerektiriyorsa true döndürür. |
| [GetFileFormatType](./getfileformattype/) | Algılanan dosya biçimini alır. |
| [GetLoadFormat](./getloadformat/) | Algılanan yükleme biçimini alır. |

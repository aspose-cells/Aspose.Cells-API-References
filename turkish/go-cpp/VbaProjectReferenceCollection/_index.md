---
title: "VbaProjectReferenceCollection Sınıfı"
linktitle: "VbaProjectReferenceCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "VbaProjectReferenceCollection sınıfı. Go'da vbaprojectreferencecollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/vbaprojectreferencecollection/
---

## VbaProjectReferenceCollection class

VBA projesinin tüm referanslarını temsil eder.

```go

type VbaProjectReferenceCollection struct  {
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
| [Get](./get/) | Listedeki referansı indeks ile al. |
| [AddRegisteredReference](./addregisteredreference/) | Bir Automation tip kitaplığına referans ekle. |
| [AddControlReferernce](./addcontrolreferernce/) | Twiddled tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekle. |
| [AddProjectReferernce](./addprojectreferernce/) | Harici bir VBA projesine referans ekler. |
| [Copy](./copy/) | Diğer VBA projesinden referansları kopyalar. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |

---
title: "ProtectedRange Sınıfı"
linktitle: "ProtectedRange"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ProtectedRange sınıfı. Go'da protectedrange'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/protectedrange/
---

## ProtectedRange class

Sayfa koruması AÇIK olduğunda düzenlemeye izin verilen belirli bir aralık.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | Aralık başlığını alır. Bu, adlandırılmış aralık tanımı olarak değil, bir tanımlayıcı olarak kullanılır. |
| [SetName](./setname/) | Aralık başlığını alır. Bu, adlandırılmış aralık tanımı olarak değil, bir tanımlayıcı olarak kullanılır. |
| [GetCellArea](./getcellarea/) | Korunacak hücre alanını temsil eden CellArea nesnesini alır. |
| [GetAreas](./getareas/) | Tüm referans verilen alanları alır. |
| [AddArea](./addarea/) | Bu nesneye bir referans alanı ekler |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Çalışma sayfasının şifreyle korunup korunmadığını gösterir. |
| [GetPassword](./getpassword/) | Aralığı korumak için şifreyi temsil eder. |
| [SetPassword](./setpassword/) | Aralığı korumak için şifreyi temsil eder. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre girmeden bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Güvenlik tanımlayıcısı, bu aralığa erişmek için şifre girmeden bu aralığı düzenleyebilecek kullanıcı hesaplarını tanımlar. |

---
title: "SignatureLine Sınıfı"
linktitle: "SignatureLine"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SignatureLine sınıfı. Go'da signatureline'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/signatureline/
---

## SignatureLine class

İmza satırını temsil eder.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetId](./getid/) | Bu imza satırı için tanımlayıcıyı alır veya ayarlar. |
| [SetId](./setid/) | Bu imza satırı için tanımlayıcıyı alır veya ayarlar. |
| [GetProviderId](./getproviderid/) | İmza sağlayıcısının kimliğini alır veya ayarlar. |
| [SetProviderId](./setproviderid/) | İmza sağlayıcısının kimliğini alır veya ayarlar. |
| [GetSigner](./getsigner/) | İmzayı atanı alır veya ayarlar. |
| [SetSigner](./setsigner/) | İmzayı atanı alır veya ayarlar. |
| [GetTitle](./gettitle/) | Şarkıcının başlığını alır veya ayarlar. |
| [SetTitle](./settitle/) | Şarkıcının başlığını alır veya ayarlar. |
| [GetEmail](./getemail/) | Şarkıcının e-posta adresini alır veya ayarlar. |
| [SetEmail](./setemail/) | Şarkıcının e-posta adresini alır veya ayarlar. |
| [IsLine](./isline/) | Bir imza satırı olup olmadığını gösterir. |
| [SetIsLine](./setisline/) | Bir imza satırı olup olmadığını gösterir. |
| [GetAllowComments](./getallowcomments/) | Yorumların eklenip eklenemeyeceğini gösterir. |
| [SetAllowComments](./setallowcomments/) | Yorumların eklenip eklenemeyeceğini gösterir. |
| [GetShowSignedDate](./getshowsigneddate/) | İmza tarihinin gösterilip gösterilmeyeceğini belirtir. |
| [SetShowSignedDate](./setshowsigneddate/) | İmza tarihinin gösterilip gösterilmeyeceğini belirtir. |
| [GetInstructions](./getinstructions/) | İmzalama sırasında kullanıcıya gösterilen metni alır veya ayarlar. |
| [SetInstructions](./setinstructions/) | İmzalama sırasında kullanıcıya gösterilen metni alır veya ayarlar. |
| [GetSignatureLineType](./getsignaturelinetype/) | İmza türünü alır veya ayarlar. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri {0000000000-0000-0000-0000-0000000000} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle {000CD6A4-0000-0000-C000-000000000046} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değerinin genellikle kullanıcı tarafından ayarlanması gerekir. Bu değer, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir. |
| [SetSignatureLineType](./setsignaturelinetype/) | İmza türünü alır veya ayarlar. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri {0000000000-0000-0000-0000-0000000000} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle {000CD6A4-0000-0000-C000-000000000046} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değerinin genellikle kullanıcı tarafından ayarlanması gerekir. Bu değer, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir. |

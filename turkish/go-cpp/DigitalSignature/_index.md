---
title: "DigitalSignature Sınıfı"
linktitle: "DigitalSignature"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DigitalSignature sınıfı. Go'da digitalsignature nesnesini kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/digitalsignature/
---

## DigitalSignature class

Dosyadaki imza.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | DigitalSignature yapıcısı. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | DigitalSignature yapıcısı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetComments](./getcomments/) | İmzanın amacı. |
| [SetComments](./setcomments/) | İmzanın amacı. |
| [GetSignTime](./getsigntime/) | Belgenin imzalandığı zaman. |
| [SetSignTime](./setsigntime/) | Belgenin imzalandığı zaman. |
| [GetId](./getid/) | Belge içeriğinde saklanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir. |
| [SetId](./setid/) | Belge içeriğinde saklanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir. |
| [GetText](./gettext/) | Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş. |
| [SetText](./settext/) | Dijital imzada gerçek imzanın metnini belirtir. Varsayılan değer Boş. |
| [GetImage](./getimage/) | Dijital imza için bir görüntü belirtir. Varsayılan değer null. |
| [SetImage](./setimage/) | Dijital imza için bir görüntü belirtir. Varsayılan değer null. |
| [GetProviderId](./getproviderid/) | İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID. |
| [SetProviderId](./setproviderid/) | İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID. |
| [IsValid](./isvalid/) | Bu dijital imza geçerli ve belge değiştirilmemişse, bu değer doğru olacaktır. |
| [GetXAdESType](./getxadestype/) | XAdES türü. Varsayılan değer None (XAdES kapalı). |
| [SetXAdESType](./setxadestype/) | XAdES türü. Varsayılan değer None (XAdES kapalı). |

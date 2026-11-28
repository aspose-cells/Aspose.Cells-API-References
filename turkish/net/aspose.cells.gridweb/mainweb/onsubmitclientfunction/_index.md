---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MainWeb özelliği. Kontrol istemci tarafında gönderilmeden önce çağrılacak istemci işlevini alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnSubmitarg cancelEdit  return true Arg, sunucuya gönderilecek komutu içeren gönderim argümanıdır. cancelEdit, kontrolün gönderimden önce kullanıcı girişini iptal edip etmediğini gösteren boolean bir değerdir. İşlev true döndürürse kontrol gönderime devam eder. Not: Olayı tetikleyen ızgara kontrolunu işaret etmek için istemci işlevinde this işaretçisini kullanabilirsiniz"
type: docs
url: /tr/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

İstemci tarafında kontrol gönderilmeden önce çağrılacak istemci işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnSubmit(arg, cancelEdit) { return true;} Arg, gönderim argümanıdır ve sunucuya gönderilecek komutu içerir. cancelEdit, kontrolün gönderimden önce kullanıcı girdisini iptal edip etmediğini gösteren boolean değerdir. İşlev true döndürürse kontrol gönderime devam eder. Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Ayrıca Bakınız

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)



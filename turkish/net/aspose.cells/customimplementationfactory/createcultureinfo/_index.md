---
title: CreateCultureInfo
second_title: Aspose.Cells for .NET API Referansı
description: Verilen kimliğe göre bir CultureInfo oluşturun.
type: docs
weight: 20
url: /tr/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Verilen kimliğe göre bir CultureInfo oluşturun.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| lcid | Int32 |  |

### Geri dönüş değeri

CultureInfo örneği.

### Notlar

Bu uygulama şu durumlar için kullanışlıdır: 1. Bazı kültürler kullanıcının ortamı tarafından desteklenmeyebilir ve gerekli CultureInfo'nun verilen tanımlayıcıyla oluşturulması İstisnaya neden olabilir. İstisnadan kaçınmak için kullanıcı, aşağıdakiler için geçerli bir CultureInfo örneği sağlamak için bu yöntemi geçersiz kılabilir. desteklenmeyen one. 2. Kullanıcı, biçimlendirme için beklenen sonucu almak üzere bazı kültürler için bazı özel özellikler belirtmek isteyebilir. Bu amaçla kullanıcı, CultureInfo örneğine kullanıcı tarafından belirlenen özellikler sağlamak için bu yöntemi geçersiz kılabilir. döndürülen CultureInfo örneği, biçimlendirilmiş sonucu etkileyebilir. Yanlış ise, döndürülen CultureInfo örneğinin bazı özellikleri, farklı senaryoların biçimlendirme gereksinimlerine göre yerleşik biçimlendirme motorumuz tarafından geçersiz kılınabilir. Bu doğruysa, herhangi bir özelliğini değiştirin ve değerleri doğrudan biçimlendirmek için kullanın. Yani, kullanıcının özel bir özelliği varsa döndürülen CultureInfo örneği için onaylanmış özel özellikler, lütfen UseUserOverride'ın true olduğundan emin olun.

### Ayrıca bakınız

* class [CustomImplementationFactory](../../customimplementationfactory)
* ad alanı [Aspose.Cells](../../customimplementationfactory)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
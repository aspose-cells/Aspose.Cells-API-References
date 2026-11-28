---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomImplementationFactory yöntemi. Verilen kimlik ile bir CultureInfo oluşturur"
type: docs
url: /tr/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Verilen kimliğe göre bir CultureInfo oluşturun.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| lcid | Int32 |  |

### Dönüş Değeri

CultureInfo örneği.

### Açıklamalar

Bu uygulama şu durumlar için yararlıdır: 1. Bazı kültürler kullanıcının ortamı tarafından desteklenmeyebilir ve verilen tanımlayıcı ile gerekli CultureInfo oluşturulması Exception oluşturabilir. İstisnayı önlemek için kullanıcı bu yöntemi geçersiz kılarak desteklenmeyen kültür için geçerli bir CultureInfo örneği sağlayabilir. 2. Kullanıcı, bazı kültürler için biçimlendirme sonucunu beklenen şekilde almak amacıyla özel özellikler belirlemek isteyebilir. Bu amaçla kullanıcı bu yöntemi geçersiz kılarak kullanıcı tarafından belirtilen özelliklere sahip bir CultureInfo örneği sağlayabilir. Lütfen döndürülen CultureInfo örneğinin UseUserOverride özelliğinin biçimlendirilmiş sonucu etkileyebileceğini unutmayın. Eğer false ise, döndürülen CultureInfo örneğinin bazı özellikleri, farklı senaryoların biçimlendirme gereksinimlerine göre yerleşik biçimlendirme motorumuz tarafından geçersiz kılınabilir. Eğer true ise, hiçbir özelliğini değiştirmeyecek ve değerleri doğrudan biçimlendirmek için kullanacağız. Bu nedenle, kullanıcı döndürülen CultureInfo örneği için özel özellikler belirlemişse, UseUserOverride değerinin true olduğundan emin olun.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // CustomImplementationFactory bir örneği oluşturun
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Geçerli bir LCID (İngilizce - Amerika Birleşik Devletleri için 1033) ile CreateCultureInfo'i çağırın
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Sonuçları görüntüleyin
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // CellsHelper içinde fabrikanın ayarlanmasını gösterin
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



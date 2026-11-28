---
title: "WebExtensionPropertyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionPropertyCollection özelliği. Web uzantısının özelliğini indeksle alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Web uzantısının özelliğini indeksle alır.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Web uzantısının özelliği.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir web uzantısı özelliği koleksiyonu oluştur
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Bazı özellikler ekleyin
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Özelliklere Item dizinleyicisiyle eriş
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Koleksiyon aracılığıyla özellik değerlerini değiştirin
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Değişiklikleri gösterin
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Çalışma kitabını kaydedin (ancak web uzantısı özellikleri uygun ayar olmadan kaydedilen dosyada görünmez)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Web uzantısının özelliğini alır.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Özelliğin adı. |

### Dönüş Değeri

Web uzantısının özelliği.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir web uzantısı özelliği koleksiyonu oluştur
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Koleksiyona özellikler ekle.
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Özelliklere Item dizinleyicisini kullanarak erişin
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Özellik değerlerini değiştirin (not: Item yalnızca okunur, bu yüzden Add/Remove kullanmamız gerekir)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Güncellenmiş değeri göster
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)



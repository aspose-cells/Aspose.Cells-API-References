---
title: "SmartTagPropertyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagPropertyCollection özelliği. Bir SmartTagProperty nesnesi alır"
type: docs
url: /tr/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Bir [`SmartTagProperty`](../../smarttagproperty/) nesnesi alır.

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks |

### Dönüş Değeri

Bir [`SmartTagProperty`](../../smarttagproperty/) nesnesi döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir akıllı etiket özelliği koleksiyonu oluşturun.
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Koleksiyona özellikler ekle.
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Özelliklere Item dizinleyicisiyle eriş
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Mevcut özellik değerlerini gösterin.
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Not: Item özelliği yalnızca okunur, bu yüzden ona doğrudan değer atayamayız.
            // Bunun yerine, döndürülen SmartTagProperty nesnelerinin özelliklerini değiştirebiliriz.
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Güncellenmiş değerleri gösterin.
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Çalışma kitabını kaydedin (ancak akıllı etiketler basit bir kayıtta görünür şekilde depolanmaz).
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Özelliğin adıyla bir [`SmartTagProperty`](../../smarttagproperty/) nesnesi alır.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Özelliğin adı. |

### Dönüş Değeri

Bir [`SmartTagProperty`](../../smarttagproperty/) nesnesi döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir akıllı etiket ayarı oluşturun ve bir akıllı etiket ekleyin.
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Akıllı etiketi ve özelliklerini alın.
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Item özelliğini göstermek için bazı özellikler ekleyin.
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Özelliklere Item indeksleyicisini (indeksle) kullanarak erişin.
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Özellik değerlerini göster
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Çalışma kitabını kaydedin
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)



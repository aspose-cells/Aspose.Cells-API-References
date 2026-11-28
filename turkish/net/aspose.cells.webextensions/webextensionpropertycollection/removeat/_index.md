---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionPropertyCollection yöntemi. Özelliği adına göre kaldırır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Özelliği ada göre kaldırır.

```csharp
public void RemoveAt(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir web uzantısı özelliği koleksiyonu oluştur
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Koleksiyona bazı özellikler ekle
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // RemoveAt yöntemini string parametresiyle çağır
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Kalan özellikleri göster
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)



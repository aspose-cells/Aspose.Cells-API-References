---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentPropertyCollection yöntemi. Belirtilen dizindeki bir özelliği kaldırır"
type: docs
url: /tr/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Belirtilen dizindeki bir özelliği kaldırır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Sıfır tabanlı dizin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel belge özelliklerine erişin (yerleşik olanların yerine)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Kaldırmayı göstermek için bazı özel özellikler ekleyin
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Kaldırmadan önce özellikleri görüntüleyin
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // 1. dizinle (ikinci özellik) RemoveAt'i çağırın
                properties.RemoveAt(1);

                // Kaldırma işleminden sonra özellikleri görüntüleyin
                Console.WriteLine("\nProperties after removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error: Index out of range. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



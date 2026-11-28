---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookMetadata özelliği. Elektronik tabloyun tüm yerleşik belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Bir [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür; bu koleksiyon, elektronik tablonun tüm yerleşik belge özelliklerini temsil eder.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Çalışma kitabını bir dosyaya kaydedin
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // Belge özellikleri için meta veri seçenekleri oluştur
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Çalışma kitabı meta verisini başlat
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // Yerleşik belge özelliklerine eriş (yalnızca okuma)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // Bazı yerleşik belge özelliklerini göster
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // Bazı yerleşik özellikleri değiştir (okuma-yazma olduğu için)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // Meta veri değişikliklerini kaydet
                metadata.Save(filePath);

                Console.WriteLine("\nBuilt-in properties have been updated and saved successfully.");
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

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)



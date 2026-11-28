---
title: "Sınıf WorkbookMetadata"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metadata.WorkbookMetadata sınıfı. Meta verileri temsil eder"
type: docs
url: /tr/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Meta verileri temsil eder.

```csharp
public class WorkbookMetadata
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Meta veri nesnesini oluştur. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Meta veri nesnesini oluştur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Elektronik tablonun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Meta verinin seçeneklerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Değiştirilmiş meta veriyi akışa kaydet. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Değiştirilmiş meta veriyi dosyaya kaydet. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // MetadataOptions örneği oluştur
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Dosya adı ve seçeneklerle WorkbookMetadata örneği oluştur
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Özel bir belge özelliği ekle
            meta.CustomDocumentProperties.Add("test", "test");

            // Meta veriyi yeni bir dosyaya kaydet
            meta.Save("WorkbookMetadataExample.xlsx");

            // Yerleşik belge özelliklerine erişimi göster
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Özel belge özelliklerine erişimi göster
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Meta veriyi bir akışa kaydet
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)



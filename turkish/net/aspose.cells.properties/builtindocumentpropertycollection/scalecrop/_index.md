---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BuiltInDocumentPropertyCollection özelliği. Belge küçük resminin görüntüleme modunu gösterir"
type: docs
url: /tr/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Belge küçük resminin görüntüleme modunu gösterir.

```csharp
public bool ScaleCrop { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özelliklerine eriş
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // ScaleCrop özelliğini ayarlayın
            properties.ScaleCrop = true;
            
            // ScaleCrop özelliği değerini görüntüleyin
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)



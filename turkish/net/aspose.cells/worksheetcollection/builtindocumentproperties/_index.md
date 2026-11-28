---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Bir [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür; bu koleksiyon, elektronik tablonun tüm yerleşik belge özelliklerini temsil eder.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Açıklamalar

Yeni bir özellik, yerleşik belge özellikleri listesine eklenemez. Yalnızca bir yerleşik özelliği alabilir ve değerini değiştirebilirsiniz. Aşağıda yerleşik özelliklerin ad listesi verilmiştir:

Title

Subject

Author

Keywords

Comments

Template

Last Author

Revision Number

Application Name

Last Print Date

Creation Date

Last Save Time

Total Editing Time

Number of Pages

Kelime Sayısı

Karakter Sayısı

Güvenlik

Kategori

Biçim

Yönetici

Şirket

Bayt Sayısı

Satır Sayısı

Paragraf Sayısı

Slayt Sayısı

Not Sayısı

Gizli Slayt Sayısı

Multimedya Klip Sayısı

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### Ayrıca Bakınız

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



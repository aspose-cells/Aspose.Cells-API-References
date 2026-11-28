---
title: "WorksheetCollection.Names"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır.

```csharp
public NameCollection Names { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Adında özel karakterler içeren bir çalışma sayfası ekleyin
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Names koleksiyonuna erişin
            NameCollection names = workbook.Worksheets.Names;
            
            // Yeni adlandırılmış bir aralık ekleyin
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Aralık referansını ayarlayın ve kullanımını gösterin
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Adlandırılmış aralık özelliklerini çıktılayın
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



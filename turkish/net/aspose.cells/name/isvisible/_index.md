---
title: "Name.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. İsmin görünür olup olmadığını belirtir"
type: docs
url: /tr/net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Adın görünür olup olmadığını gösterir.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görünür bir adlandırılmış aralık oluştur
            int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
            Name visibleName = workbook.Worksheets.Names[visibleIndex];
            visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
            visibleName.IsVisible = true;
            
            // Gizli bir adlandırılmış aralık oluştur
            int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
            Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
            hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
            hiddenName.IsVisible = false;
            
            // IsVisible özelliğini göster
            Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
            Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
            
            // Çalışma kitabını kaydedin
            workbook.Save("NameVisibilityDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



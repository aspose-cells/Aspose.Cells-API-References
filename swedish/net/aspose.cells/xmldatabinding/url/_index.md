---
title: "XmlDataBinding.Url"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlDataBinding-egenskap. Hämtar käll-url för denna databindning"
type: docs
url: /sv/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Hämtar käll‑URL för denna databindning.

```csharp
public string Url { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till två arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Lägg till listobjekt och XML-kartor
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Hämta XML-databindnings-URL:er (Url är skrivskyddad)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Visa URL:erna
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Spara arbetsboken
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Se även

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



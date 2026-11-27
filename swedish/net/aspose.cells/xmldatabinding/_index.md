---
title: "Klass XmlDataBinding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XmlDataBinding-klass. Representerar information om XML‑databindning"
type: docs
url: /sv/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Representerar information om Xml Data Binding.

```csharp
public class XmlDataBinding
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Hämtar käll‑URL för denna databindning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett listobjekt som kommer att använda XML-databindning
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Hämta XML-databindningsinformationen (detta skulle vanligtvis ställas in när XML-data importeras)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Visa URL:en för XML-datakällan (skrivskyddad egenskap)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Obs: I ett verkligt scenario skulle URL:en sättas när XML-data importeras
            // För demonstrationsändamål visar vi hur man får åtkomst till egenskapen

            // Spara arbetsboken
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



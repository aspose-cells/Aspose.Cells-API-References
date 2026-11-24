---
title: "XmlDataBinding.Url"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlDataBinding-Eigenschaft. Gibt die Quell-URL dieses Datenbindings zurück"
type: docs
url: /de/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Liest die Quell‑URL dieser Datenbindung.

```csharp
public string Url { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge zwei Arbeitsblätter hinzu
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Füge Listobjekte und XML-Maps hinzu
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Rufe XML-Datenbindungs-URLs ab (Url ist schreibgeschützt)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Zeige die URLs an
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Speichere die Arbeitsmappe
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



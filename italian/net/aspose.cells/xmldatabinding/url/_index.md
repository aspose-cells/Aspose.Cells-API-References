---
title: "XmlDataBinding.Url"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlDataBinding. Ottiene l'url di origine di questo binding dati"
type: docs
url: /it/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Ottiene l'url di origine di questo binding dei dati.

```csharp
public string Url { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi due fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Aggiungi oggetti elenco e mappe XML
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Ottieni gli URL del binding dati XML (Url è di sola lettura)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Visualizza gli URL
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Salva la cartella di lavoro
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



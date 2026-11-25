---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Colonna nascosta: la larghezza di questa colonna è 0 in Excel. Prima di salvare in formato html, se HtmlHiddenColDisplayType è Removethe, la colonna nascosta non verrà esportata; se il valore è Hidden, la colonna verrà esportata ma rimarrà nascosta. Il valore predefinito è Hidden"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è \"Remove\", la colonna nascosta non verrà emessa; se il valore è \"Hidden\", la colonna verrà emessa ma rimarrà nascosta. Il valore predefinito è \"Hidden\".

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Nascondi la colonna C (indice 2)
            worksheet.Cells.HideColumn(2);

            // Aggiungi alcuni dati per dimostrare
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Crea le opzioni di salvataggio HTML con diverse impostazioni di HiddenColDisplayType
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Salva con opzioni diverse
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Vedi anche

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se l'HTML di output è compatibile con dispositivi mobili. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta la compatibilità mobile
            saveOptions.IsMobileCompatible = true;

            // Salva con la compatibilità mobile abilitata
            workbook.Save("MobileCompatible.html", saveOptions);

            // Passa a non compatibile con mobile
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



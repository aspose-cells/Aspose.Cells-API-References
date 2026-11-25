---
title: "XlsSaveOptions.WpsCompatibility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsSaveOptions. Indica se rendere il file xls più compatibile con WPS"
type: docs
url: /it/net/aspose.cells/xlssaveoptions/wpscompatibility/
---
## XlsSaveOptions.WpsCompatibility property

Indica se rendere il file xls più compatibile con WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookSetting.WpsCompatibility. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Imposta le opzioni di salvataggio con compatibilità WPS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.WpsCompatibility = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output_with_wps_compatibility.xls", saveOptions);
            
            Console.WriteLine("File saved with WPS compatibility enabled.");
        }
    }
}
```

### Vedi anche

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



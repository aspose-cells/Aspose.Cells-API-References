---
title: "OoxmlSaveOptions.WpsCompatibility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Indica se rendere il file xls più compatibile con WPS"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

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
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // Crea le opzioni di salvataggio OOXML e abilita la compatibilità WPS
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // Salva la cartella di lavoro con compatibilità WPS
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



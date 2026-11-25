---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Indica se il file HTML o MHT è la preferenza di presentazione. Il valore predefinito è false. Se desideri ottenere una presentazione più bella, imposta il valore su true.

```csharp
public bool PresentationPreference { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Imposta le opzioni di salvataggio HTML con PresentationPreference
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // Salva su stream di memoria per dimostrazione
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



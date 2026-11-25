---
title: "CalculationOptions.CharacterEncoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR CODE il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da usare per tali funzioni per ottenere il risultato previsto"
type: docs
url: /it/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



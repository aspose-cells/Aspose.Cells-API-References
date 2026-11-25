---
title: "WarningInfo.WarningType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WarningInfo. Ottieni il tipo di avviso"
type: docs
url: /it/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Ottieni il tipo di avviso.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WarningInfo.Type. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e genera un avviso
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Questo genererà un avviso durante il salvataggio con funzionalità non supportate
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Salva con un formato che potrebbe generare avvisi
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Dimostra l'uso della proprietà WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Gestisci tipi di avviso specifici
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Vedi anche

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



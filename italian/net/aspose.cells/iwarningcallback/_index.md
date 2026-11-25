---
title: "Interfaccia IWarningCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.IWarningCallback. Interfaccia di callback per avvisi"
type: docs
url: /it/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Interfaccia di callback di avviso.

```csharp
public interface IWarningCallback
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Il nostro callback deve solo implementare il metodo \"Warning\". |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Implementazione del metodo Warning dall'interfaccia IWarningCallback
        public void Warning(WarningInfo warningInfo)
        {
            // Visualizza il messaggio di avviso
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta il callback di avviso
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Carica una cartella di lavoro con potenziali avvisi
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Salva la cartella di lavoro
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



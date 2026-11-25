---
title: "Protection.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Protection. Copia le informazioni di protezione"
type: docs
url: /it/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Copia le informazioni di protezione.

```csharp
public void Copy(Protection source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Protection |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea le impostazioni di protezione di origine - utilizza la protezione esistente dal foglio di lavoro
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Ottieni le impostazioni di protezione di destinazione
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Chiama il metodo Copy con il parametro Protection
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



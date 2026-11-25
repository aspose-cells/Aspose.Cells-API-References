---
title: "Worksheet.Protection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. Supporta opzioni di protezione avanzate in ExcelXP e versioni successive"
type: docs
url: /it/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. Supporta opzioni di protezione avanzate in ExcelXP e versioni successive.

```csharp
public Protection Protection { get; }
```

### Osservazioni

Questa proprietà può proteggere il foglio di lavoro in tutte le versioni del file Excel e supporta opzioni di protezione avanzate in ExcelXP e versioni successive.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accedi alle proprietà di protezione
            Protection protection = sheet.Protection;
            
            // Imposta le proprietà di protezione
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Proteggi il foglio di lavoro (usando il metodo Protect invece di impostare direttamente IsProtectedWithPassword)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Salva la cartella di lavoro
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Verifica le impostazioni di protezione
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Vedi anche

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "VbaProject.Protect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProject. Protegge o rimuove la protezione di questo progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Protegge o rimuove la protezione di questo progetto VBA.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| islockedForViewing | Booleano | indica se il progetto è bloccato per la visualizzazione. |
| password | String | Se il valore è null, rimuove la protezione di questo progetto VBA, altrimenti proietta questo progetto VBA. |

### Osservazioni

Se islockedForViewing è true, la password non può essere null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con progetto VBA
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



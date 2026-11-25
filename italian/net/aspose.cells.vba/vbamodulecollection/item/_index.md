---
title: "VbaModuleCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaModuleCollection. Ottiene VbaModule nell'elenco per indice"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Ottiene [`VbaModule`](../../vbamodule/) nell'elenco per indice.

```csharp
public VbaModule this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con progetto VBA
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Ottieni il progetto VBA esistente (VbaProject è di sola lettura)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un modulo al progetto VBA
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Accedi al modulo usando la proprietà Item
            VbaModule module = vbaProject.Modules[index];
            
            // Aggiungi del codice VBA al modulo
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Salva la cartella di lavoro
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Ottiene [`VbaModule`](../../vbamodule/) nell'elenco per nome.

```csharp
public VbaModule this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome del modulo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi modulo VBA alla cartella di lavoro
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Accedi al modulo usando la proprietà Item per nome
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // Imposta il codice VBA
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Verifica ricaricando
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Vedi anche

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



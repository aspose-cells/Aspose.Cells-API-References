---
title: "Workbook.VbaProject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene il VbaProject in un foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Ottiene il `VbaProject` in un foglio di calcolo.

```csharp
public VbaProject VbaProject { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA (VbaProject è di sola lettura, possiamo solo verificare se esiste)
            if (workbook.VbaProject == null)
            {
                // Crea un progetto VBA salvando come cartella di lavoro con macro abilitate
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Aggiungi un nuovo modulo al progetto VBA
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Recupera il modulo aggiunto e imposta il suo codice
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Salva la cartella di lavoro
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



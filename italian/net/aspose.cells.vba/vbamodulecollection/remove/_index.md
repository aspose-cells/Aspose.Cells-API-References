---
title: "VbaModuleCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaModuleCollection. Rimuove il modulo per un foglio di lavoro"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Rimuove il modulo per un foglio di lavoro.

```csharp
public void Remove(Worksheet sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| foglio | Worksheet | Il foglio di lavoro |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un modulo VBA al foglio di lavoro
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Ottieni la collezione di moduli VBA
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Chiama il metodo Remove con il parametro foglio di lavoro
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Verifica che il modulo sia stato rimosso
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Rimuovi il modulo per nome

```csharp
public void Remove(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con macro
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un nuovo modulo
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Aggiungi del codice al modulo
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Salva la cartella di lavoro
            workbook.Save("output_with_module.xlsm");
            
            // Rimuovi il modulo per nome
            vbaProject.Modules.Remove("TestModule");
            
            // Salva la cartella di lavoro dopo la rimozione
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



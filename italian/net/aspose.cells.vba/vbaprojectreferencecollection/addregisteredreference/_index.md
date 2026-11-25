---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProjectReferenceCollection. Aggiungi un riferimento a una libreria di tipi Automation"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Aggiungi un riferimento a una libreria di tipo Automation.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del riferimento. |
| libid | String | L'identificatore di una libreria di tipo Automation. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un riferimento registrato a stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



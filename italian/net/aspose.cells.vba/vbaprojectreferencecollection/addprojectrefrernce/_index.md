---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProjectReferenceCollection. Aggiunge un riferimento a un progetto VBA esterno"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Aggiunge un riferimento a un progetto VBA esterno.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del riferimento. |
| absoluteLibid | String | L'identificatore del progetto VBA di riferimento con un percorso assoluto. |
| relativeLibid | String | L'identificatore del progetto VBA di riferimento con un percorso relativo. |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo VbaProjectReferenceCollection.AddProjectReferernce(). Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Inizializza il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Aggiungi un riferimento di progetto con libid assoluti e relativi
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Visualizza il conteggio dei riferimenti
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Salva la cartella di lavoro
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



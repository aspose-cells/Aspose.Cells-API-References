---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaProjectReferenceCollection. Aggiunge un riferimento a una libreria di tipo twiddled e alla sua libreria di tipo estesa"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Aggiungi un riferimento a una libreria di tipo modificata e alla sua libreria di tipo estesa.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del riferimento. |
| libid | String | L'identificatore di una libreria di tipo Automation. |
| twiddledlibid | String | L'identificatore di una libreria di tipo twiddled |
| extendedLibid | String | L'identificatore di una libreria di tipo estesa |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo VbaProjectReferenceCollection.AddControlReferernce(). Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Aggiungi riferimento di controllo con tutti i parametri stringa
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



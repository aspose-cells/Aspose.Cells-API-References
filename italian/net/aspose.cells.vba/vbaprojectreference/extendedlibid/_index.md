---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "VbaProjectReference proprietà. Ottiene e imposta il Libid esteso del riferimento"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Ottiene e imposta il Libid esteso del riferimento.

```csharp
public string ExtendedLibid { get; set; }
```

### Osservazioni

Solo per riferimento di controllo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Inizializza il progetto VBA
                VbaProject vbaProject = workbook.VbaProject;

                // Aggiungi un riferimento di controllo per dimostrare ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Ottieni il primo riferimento
                VbaProjectReference reference = vbaProject.References[0];

                // Visualizza il valore della proprietà ExtendedLibid
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Dimostra l'impostazione di ExtendedLibid (poiché è in lettura/scrittura)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Salva la cartella di lavoro
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



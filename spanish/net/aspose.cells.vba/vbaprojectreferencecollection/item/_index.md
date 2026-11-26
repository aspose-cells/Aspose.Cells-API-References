---
title: "VbaProjectReferenceCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReferenceCollection. Obtenga la referencia en la lista por el índice"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Obtenga la referencia en la lista por el índice.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| i | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar referencias al proyecto VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Obtener la colección de referencias
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Acceder a las referencias usando la propiedad Item
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Guarda el libro de trabajo
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)



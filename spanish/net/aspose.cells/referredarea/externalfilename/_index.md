---
title: "ReferredArea.ExternalFileName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. Obtenga el nombre del archivo externo si esta es una referencia externa"
type: docs
url: /es/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Obtener el nombre del archivo externo si es una referencia externa.

```csharp
public string ExternalFileName { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con referencia externa
            Workbook wb = new Workbook();
            
            // Crear un nombre que haga referencia a un libro de trabajo externo
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Obtener el área referida
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Demostrar la propiedad ExternalFileName
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Verificar el nombre del archivo externo
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



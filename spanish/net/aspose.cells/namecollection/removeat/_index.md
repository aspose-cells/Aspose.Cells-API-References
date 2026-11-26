---
title: "NameCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Elimina el nombre en el índice específico"
type: docs
url: /es/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Elimina el nombre en el índice específico.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | índice del Name a eliminar. |

### Observaciones

Por favor, asegúrese de que el nombre no sea referenciado por otras fórmulas antes de llamar al método. Y si el nombre es referenciado, establecer Name.RefersTo como null es mejor.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Agregar nombres a la colección
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Eliminar nombre por índice
            names.RemoveAt(firstIndex);

            // Verificar la eliminación comprobando el recuento
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



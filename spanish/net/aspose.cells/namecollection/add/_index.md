---
title: "NameCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Define un nuevo nombre"
type: docs
url: /es/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Define un nuevo nombre.

```csharp
public int Add(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto a usar como nombre. |

### Valor de retorno

[`Name`](../../name/) object index.

### Observaciones

El nombre no puede incluir espacios y no puede parecer una referencia de celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Agregue un nombre con referencia de cadena
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Establezca la fórmula a la que se refiere el nombre
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Verifique y muestre los resultados
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Obtenga el rango y muestre su dirección
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



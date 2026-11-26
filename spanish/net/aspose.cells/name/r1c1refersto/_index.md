---
title: "Name.R1C1RefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Obtiene o establece una referencia R1C1 del Name"
type: docs
url: /es/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Obtiene o establece una referencia R1C1 del [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un nuevo nombre a la colección de nombres
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Establecer referencia R1C1 para el nombre
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Verificar que la referencia se haya establecido correctamente
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Guarda el libro de trabajo
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



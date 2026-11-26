---
title: "Name.RefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual."
type: docs
url: /es/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual.

```csharp
public string RefersTo { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Agregar rangos con nombre con RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Mostrar la propiedad RefersTo de los rangos con nombre
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



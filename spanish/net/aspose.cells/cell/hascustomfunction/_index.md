---
title: "Cell.HasCustomFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Verifica si hay una función personalizada no compatible en la fórmula de esta celda."
type: docs
url: /es/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Comprueba si hay una función personalizada (función no compatible) en la fórmula de esta celda.

```csharp
public bool HasCustomFunction { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar un nombre de función personalizada
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Probar con función incorporada
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Probar con función personalizada
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Probar con rango nombrado que contiene función personalizada
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Probar con función personalizada anidada
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



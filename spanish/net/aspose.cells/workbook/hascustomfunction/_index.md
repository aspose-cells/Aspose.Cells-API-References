---
title: "Workbook.HasCustomFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Detecta si hay una función personalizada usada en este libro de trabajo, como en fórmulas de celdas en nombres definidos"
type: docs
url: /es/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Detecta si hay una función personalizada utilizada en este libro de trabajo, como en la fórmula de una celda, en nombres definidos...

```csharp
public bool HasCustomFunction { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar una fórmula estándar a un nombre
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Agregar una función personalizada a un nombre
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Probar con fórmulas de celda
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Función estándar en celda
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Función personalizada en celda
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Referencia a un nombre con función personalizada
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Funciones personalizadas combinadas
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



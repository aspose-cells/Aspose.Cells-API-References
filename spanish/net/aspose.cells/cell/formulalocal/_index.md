---
title: "Cell.FormulaLocal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene la fórmula formateada según la configuración regional de la celda"
type: docs
url: /es/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Obtenga la fórmula formateada según la configuración regional de la celda.

```csharp
public string FormulaLocal { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la configuración regional predeterminada a alemán para la demostración
            workbook.Settings.Region = CountryCode.Germany;
            
            // Acceder a la celda A1
            Cell cell = worksheet.Cells["A1"];
            
            // Establecer la fórmula en formato estándar (Inglés)
            cell.Formula = "=SUM(B1:C1)";
            
            // Mostrar fórmulas en ambos formatos, estándar y local
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Establecer la fórmula en formato local (Alemán)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Mostrar las fórmulas nuevamente para mostrar la diferencia
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Demostrar GetFormula con localización
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



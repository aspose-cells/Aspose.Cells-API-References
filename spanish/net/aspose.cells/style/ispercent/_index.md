---
title: "Style.IsPercent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si el formato numérico es un formato de porcentaje"
type: docs
url: /es/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Indica si el formato numérico es un formato de porcentaje.

```csharp
public bool IsPercent { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la celda A1 y establece su valor
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Obtener el estilo de la celda
            Style style = cell.GetStyle();
            
            // Muestra el valor actual de IsPercent
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Establece el formato numérico a porcentaje (esto establecerá automáticamente IsPercent en verdadero)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Verificar que IsPercent ahora es verdadero
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Crear otra celda con un formato diferente
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Verificar que IsPercent es falso para un formato no porcentual
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Guarda el libro de trabajo
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



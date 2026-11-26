---
title: "Protection.AllowSorting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la opción de ordenación está permitida en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Representa si se permite la opción de ordenar en una hoja de cálculo protegida.

```csharp
public bool AllowSorting { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar la protección de la hoja de cálculo
            worksheet.Protect(ProtectionType.All);
            
            // Establecer propiedades de protección incluyendo AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Mostrar configuraciones de protección
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Demostrar la capacidad de ordenación
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Protection.AllowSelectingLockedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Representa si se permite al usuario seleccionar celdas bloqueadas en una hoja de cálculo protegida.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer configuraciones de protección
            Protection protection = worksheet.Protection;
            
            // Demostrar la propiedad AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Modificar la propiedad y mostrar el cambio
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Proteger la hoja de cálculo con contraseña
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Guarda el libro de trabajo
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



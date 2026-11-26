---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection property. Representa si el usuario tiene permiso para seleccionar celdas desbloqueadas en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Representa si se permite al usuario seleccionar celdas desbloqueadas en una hoja de cálculo protegida.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Protege la hoja de cálculo con todas las opciones de protección
            Protection protection = worksheet.Protection;
            
            // Establece AllowSelectingUnlockedCell en true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Aplica la protección con contraseña
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Verifique la configuración
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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



---
title: "Protection.AllowDeletingColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la eliminación de columnas está permitida en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Representa si se permite la eliminación de columnas en una hoja de cálculo protegida.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Observaciones

Las columnas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y la opción "Seleccionar celdas desbloqueadas" debe estar habilitada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar la protección de la hoja de cálculo
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Verifique la configuración
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Intentar eliminar una columna (debería funcionar ya que AllowDeletingColumn es verdadero)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Deshabilitar la eliminación de columnas
            protection.AllowDeletingColumn = false;

            // Intentar eliminar otra columna (debería fallar)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



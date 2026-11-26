---
title: "Protection.AllowDeletingRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la eliminación de filas está permitida en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Representa si se permite la eliminación de filas en una hoja de cálculo protegida.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Observaciones

Las filas que contienen las celdas a eliminar deben estar desbloqueadas cuando la hoja está protegida, y "Seleccionar celdas desbloqueadas" debe estar habilitada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer configuraciones de protección
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Proteger la hoja de cálculo
            sheet.Protect(ProtectionType.All);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Cargar el libro de trabajo guardado para verificar la configuración
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Verificar AllowDeletingRow y otras propiedades
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



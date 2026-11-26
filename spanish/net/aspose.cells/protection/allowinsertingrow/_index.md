---
title: "Protection.AllowInsertingRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la inserción de filas está permitida en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Representa si se permite la inserción de filas en una hoja de cálculo protegida

```csharp
public bool AllowInsertingRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la configuración de protección
            Protection protection = worksheet.Protection;

            // Habilitar la inserción de filas mientras está protegido
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Intentar insertar una fila (debería funcionar ya que AllowInsertingRow es verdadero)
            worksheet.Cells.InsertRow(0);

            // Guarda el libro de trabajo
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



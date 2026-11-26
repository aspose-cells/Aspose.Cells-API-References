---
title: "Protection.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection method. Copia la información de protección"
type: docs
url: /es/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Copiar información de protección.

```csharp
public void Copy(Protection source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Protection |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea la configuración de protección de origen - usa la protección existente de la hoja de cálculo
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Obtener la configuración de protección del objetivo
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Llamar al método Copy con el parámetro Protection
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



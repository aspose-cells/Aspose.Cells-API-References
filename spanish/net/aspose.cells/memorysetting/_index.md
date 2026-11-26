---
title: "Enum MemorySetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.MemorySetting. Modos de uso de memoria para el modelo de datos de celdas"
type: docs
url: /es/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Modos de uso de memoria para el modelo de datos de celdas.

```csharp
public enum MemorySetting
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Normal | `0` | Modo predeterminado para el modelo de celdas. |
| MemoryPreference | `1` | Se prefiere el rendimiento de memoria. |
| FileCache | `2` | Se prefiere el rendimiento de memoria y usar un archivo en lugar de memoria para mantener los datos de las celdas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establezca la opción de uso de memoria a MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Cree una hoja de cálculo y agregue algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Guarda el libro de trabajo
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



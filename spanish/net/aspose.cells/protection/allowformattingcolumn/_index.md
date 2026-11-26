---
title: "Protection.AllowFormattingColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si el formato de columnas está permitido en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowformattingcolumn/
---
## Protection.AllowFormattingColumn property

Representa si se permite el formato de columnas en una hoja de cálculo protegida

```csharp
public bool AllowFormattingColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la configuración de protección
            Protection protection = worksheet.Protection;

            // Establecer la propiedad AllowFormattingColumn
            protection.AllowFormattingColumn = true;

            // Verificar e imprimir el valor de la propiedad
            Console.WriteLine("AllowFormattingColumn: " + protection.AllowFormattingColumn);

            // Demostrar la configuración de múltiples propiedades de protección
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingRow = true;

            // Llamar al método de cálculo de banderas
            int protectionFlags = CalculateProtectionFlags(protection);
            Console.WriteLine("Protection Flags: 0x" + protectionFlags.ToString("X4"));
        }

        private static int CalculateProtectionFlags(Protection protection)
        {
            int flag = 0;
            if (protection.AllowDeletingColumn) { flag |= 0x0001; }
            if (protection.AllowDeletingRow) { flag |= 0x0002; }
            if (protection.AllowEditingContent) { flag |= 0x0004; }
            if (protection.AllowEditingObject) { flag |= 0x0008; }
            if (protection.AllowEditingScenario) { flag |= 0x0010; }
            if (protection.AllowFiltering) { flag |= 0x0020; }
            if (protection.AllowFormattingCell) { flag |= 0x0040; }
            if (protection.AllowFormattingColumn) { flag |= 0x0080; }
            if (protection.AllowFormattingRow) { flag |= 0x0100; }
            if (protection.AllowInsertingColumn) { flag |= 0x0200; }
            if (protection.AllowInsertingHyperlink) { flag |= 0x0400; }
            if (protection.AllowInsertingRow) { flag |= 0x0800; }
            if (protection.AllowSelectingLockedCell) { flag |= 0x1000; }
            if (protection.AllowSelectingUnlockedCell) { flag |= 0x2000; }
            if (protection.AllowSorting) { flag |= 0x4000; }
            if (protection.AllowUsingPivotTable) { flag |= 0x8000; }
            return flag;
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



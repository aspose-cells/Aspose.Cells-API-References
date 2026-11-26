---
title: "Enumeración ProtectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ProtectionType enumeración. Representa el tipo de protección del libro/hoja de cálculo"
type: docs
url: /es/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Representa el tipo de protección del libro/hoja de cálculo.

```csharp
public enum ProtectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `0` | Representa proteger todo. |
| Contents | `1` | Representa proteger el contenido, usado en la protección de la hoja. |
| Objects | `2` | Representa proteger los objetos, usado en la protección de la hoja. |
| Scenarios | `3` | Representa proteger los escenarios, usado en la protección de la hoja. |
| Structure | `4` | Representa proteger la estructura, usado en la protección del libro. |
| Windows | `5` | Representa proteger la ventana, usado en la protección del libro. |
| None | `6` | Representa sin protección. Sólo para la propiedad Reading. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteger la hoja de cálculo con todos los tipos de protección
            worksheet.Protect(ProtectionType.All);
            
            // Demostrar el acceso a las propiedades de protección
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Desproteger la hoja de cálculo
            worksheet.Unprotect();
            
            // Proteger con tipos de protección específicos
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



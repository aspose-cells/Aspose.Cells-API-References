---
title: "Clase Protection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Protection. Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/protection/
---
## Protection class

Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo.

```csharp
public class Protection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Representa si se permite la eliminación de columnas en una hoja de cálculo protegida. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Representa si se permite la eliminación de filas en una hoja de cálculo protegida. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Representa si se permite al usuario usar un AutoFiltro que se creó antes de que la hoja fuera protegida. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Representa si se permite el formato de celdas en una hoja de cálculo protegida. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Representa si se permite el formato de columnas en una hoja de cálculo protegida |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Representa si se permite el formato de filas en una hoja de cálculo protegida |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Representa si se permite la inserción de columnas en una hoja de cálculo protegida |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Representa si se permite la inserción de hipervínculos en una hoja de cálculo protegida |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Representa si se permite la inserción de filas en una hoja de cálculo protegida |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Representa si se permite al usuario seleccionar celdas bloqueadas en una hoja de cálculo protegida. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Representa si se permite al usuario seleccionar celdas desbloqueadas en una hoja de cálculo protegida. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Representa si se permite la opción de ordenar en una hoja de cálculo protegida. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Representa si se permite al usuario manipular tablas dinámicas en una hoja de cálculo protegida. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Indica si la hoja de cálculo está protegida con contraseña. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Representa la contraseña para proteger la hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Copiar información de protección. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Obtiene el hash de la contraseña actual. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Verifica la contraseña. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la configuración de protección de la hoja de cálculo
            Protection protection = worksheet.Protection;

            // Estableciendo varias propiedades de protección
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Comprobando si la hoja de cálculo está protegida con una contraseña
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Guardando el libro de trabajo
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



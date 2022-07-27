---
title: Protection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa los distintos tipos de opciones de protección disponibles para una hoja de trabajo.
type: docs
weight: 4910
url: /es/net/aspose.cells/protection/
---
## Protection class

Representa los distintos tipos de opciones de protección disponibles para una hoja de trabajo.

```csharp
public class Protection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn) { get; set; } | Representa si se permite la eliminación de columnas en una hoja de cálculo protegida. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow) { get; set; } | Representa si se permite la eliminación de filas en una hoja de trabajo protegida. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent) { get; set; } | Representa si el usuario puede editar el contenido de las celdas bloqueadas en una hoja de trabajo protegida. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject) { get; set; } | Representa si el usuario puede manipular objetos de dibujo en una hoja de trabajo protegida. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario) { get; set; } | Representa si el usuario puede editar escenarios en una hoja de trabajo protegida. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering) { get; set; } | Representa si el usuario puede utilizar un Autofiltro que se creó antes de proteger la hoja. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell) { get; set; } | Representa si se permite el formato de celdas en una hoja de cálculo protegida. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn) { get; set; } | Representa si se permite el formato de columnas en una hoja de trabajo protegida |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow) { get; set; } | Representa si se permite el formato de filas en una hoja de trabajo protegida |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn) { get; set; } | Representa si se permite la inserción de columnas en una hoja de trabajo protegida |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink) { get; set; } | Representa si se permite la inserción de hipervínculos en una hoja de trabajo protegida |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow) { get; set; } | Representa si se permite la inserción de filas en una hoja de cálculo protegida |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell) { get; set; } | Representa si el usuario puede seleccionar celdas bloqueadas en una hoja de trabajo protegida. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell) { get; set; } | Representa si el usuario puede seleccionar celdas desbloqueadas en una hoja de trabajo protegida. |
| [AllowSorting](../../aspose.cells/protection/allowsorting) { get; set; } | Representa si la opción de clasificación está permitida en una hoja de trabajo protegida. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable) { get; set; } | Representa si el usuario puede manipular tablas dinámicas en una hoja de trabajo protegida. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword) { get; } | Indica si las hojas de trabajo están protegidas con contraseña. |
| [Password](../../aspose.cells/protection/password) { get; set; } | Representa la contraseña para proteger la hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy)(Protection) | Información de protección contra copia. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash)() | Obtiene el hash de la contraseña actual. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword)(string) | Verifica contraseña. |

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

Worksheet worksheet = workbook.Worksheets[0];
// Permitiendo a los usuarios seleccionar celdas bloqueadas de la hoja de trabajo
worksheet.Protection.AllowSelectingLockedCell = true;
// Permitiendo a los usuarios seleccionar celdas desbloqueadas de la hoja de trabajo
worksheet.Protection.AllowSelectingUnlockedCell = true;  

[Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Permitir a los usuarios seleccionar celdas bloqueadas de la hoja de trabajo
worksheet.Protection.AllowSelectingLockedCell = True
'Permitir a los usuarios seleccionar celdas desbloqueadas de la hoja de trabajo
worksheet.Protection.AllowSelectingUnlockedCell = True
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

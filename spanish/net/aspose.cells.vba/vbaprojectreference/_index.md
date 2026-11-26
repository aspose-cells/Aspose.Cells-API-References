---
title: "Clase VbaProjectReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Vba.VbaProjectReference. Representa la referencia del proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Representa la referencia del proyecto VBA.

```csharp
public class VbaProjectReference
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Obtiene y establece el Libid extendido de la referencia. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Obtiene y establece el Libid de la referencia. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Obtiene y establece el nombre de la referencia. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Obtiene y establece el identificador del proyecto VBA referenciado con una ruta relativa. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Obtiene y establece el Libid manipulado de la referencia. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Obtiene el tipo de esta referencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Ejemplos

```csharp

[C#]

//Instanciando un objeto Workbook
Workbook workbook = new Workbook();
 // Inicializar proyecto VBA.
VbaProject vbaProject = workbook.VbaProject;
// Agregar referencia de proyecto VBA
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Guardando el archivo Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### Ver también

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)



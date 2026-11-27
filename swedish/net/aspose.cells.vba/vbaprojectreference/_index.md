---
title: "Klass VbaProjectReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaProjectReference-klass. Representerar referensen till VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Representerar referensen till VBA‑projektet.

```csharp
public class VbaProjectReference
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Hämtar och anger det utökade Libid för referensen. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Hämtar och anger Libid för referensen. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Hämtar och anger namnet på referensen. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Hämtar och anger identifieraren för det refererade VBA-projektet med en relativ sökväg. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Hämtar och anger det justerade Libid för referensen. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Hämtar typen för denna referens. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Exempel

```csharp

[C#]

//Instansiering av ett Workbook-objekt
Workbook workbook = new Workbook();
 // Initiera VBA-projekt.
VbaProject vbaProject = workbook.VbaProject;
// Lägg till vba-projektreferens
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Sparar Excel-filen
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

### Se även

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)



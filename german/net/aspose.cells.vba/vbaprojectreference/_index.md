---
title: "Klasse VbaProjectReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaProjectReference Klasse. Stellt die Referenz eines VBA‑Projekts dar"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Stellt die Referenz des VBA‑Projekts dar.

```csharp
public class VbaProjectReference
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Ermittelt und setzt die erweiterte Libid der Referenz. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Ermittelt und setzt die Libid der Referenz. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Ermittelt und setzt den Namen der Referenz. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Ermittelt und setzt den Bezeichner des referenzierten VBA‑Projekts mit einem relativen Pfad. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Ermittelt und setzt die manipulierte Libid der Referenz. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Ermittelt den Typ dieser Referenz. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
 // Initialisiert VBA-Projekt.
VbaProject vbaProject = workbook.VbaProject;
// VBA-Projektreferenz hinzufügen
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Die Excel-Datei speichern
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

### Siehe auch

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)



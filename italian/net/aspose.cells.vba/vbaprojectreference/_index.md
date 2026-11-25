---
title: "Classe VbaProjectReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Vba.VbaProjectReference. Rappresenta il riferimento del progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Rappresenta il riferimento del progetto VBA.

```csharp
public class VbaProjectReference
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Ottiene e imposta il Libid esteso del riferimento. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Ottiene e imposta il Libid del riferimento. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Ottiene e imposta il nome del riferimento. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Ottiene e imposta l'identificatore del progetto VBA di riferimento con un percorso relativo. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Ottiene e imposta il Libid modificato del riferimento. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Ottiene il tipo di questo riferimento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Esempi

```csharp

[C#]

//Istanziare un oggetto Workbook
Workbook workbook = new Workbook();
 // Inizializza il progetto VBA.
VbaProject vbaProject = workbook.VbaProject;
// Aggiungi riferimento al progetto VBA
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Salvataggio del file Excel
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

### Vedi anche

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)



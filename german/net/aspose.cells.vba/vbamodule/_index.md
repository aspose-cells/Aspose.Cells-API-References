---
title: VbaModule
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert das Modul im VBA-Projekt.
type: docs
weight: 6240
url: /de/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Repräsentiert das Modul im VBA-Projekt.

```csharp
public class VbaModule
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Codes](../../aspose.cells.vba/vbamodule/codes) { get; set; } | Holt und setzt die Codes des Moduls. |
| [Name](../../aspose.cells.vba/vbamodule/name) { get; set; } | Ruft den Namen des Moduls ab und legt ihn fest. |
| [Type](../../aspose.cells.vba/vbamodule/type) { get; } | Ruft den Typ des Moduls ab. |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
 // VBA-Projekt initialisieren.
VbaProject vbaProject = workbook.VbaProject; 
// Neues Modul hinzufügen.
int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
// VBA-Modul abrufen
VbaModule vbaModule = vbaProject.Modules[index];
// Codes setzen
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
//Speichern der Excel-Datei
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
'VBA-Projekt initialisieren.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Fügen Sie ein neues Modul hinzu.
Dim index as Integer = vbaProject.Modules.Add(VbaModuleType.Class, "test")
'Holen Sie sich das vba-Modul
Dim vbaModule as VbaModule = vbaProject.Modules(index)
'Codes festlegen
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
'Speichern der Excel-Datei
workbook.Save("book1.xlsm")
```

### Siehe auch

* namensraum [Aspose.Cells.Vba](../../aspose.cells.vba)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
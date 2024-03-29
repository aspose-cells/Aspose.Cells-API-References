---
title: Class VbaProject
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Vba.VbaProject class. Represents the VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Represents the VBA project.

```csharp
public class VbaProject
```

## Properties

| Name | Description |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Gets certificate raw data if this VBA project is signed. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Gets and sets the encoding of VBA project. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | Indicates whether this VBA project is locked for viewing. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Indicates whether this VBA project is protected. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Indicates whether VBAcode is signed or not. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Indicates whether the signature of VBA project is valid or not. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Gets all [`VbaModule`](../vbamodule/) objects. |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Gets and sets the name of the VBA project. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Gets all references of VBA project. |

## Methods

| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Copy VBA project from other file. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Protects or unprotects this VBA project. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Sign this VBA project by a DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Validates protection password. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
 // Init VBA project.
VbaProject vbaProject = workbook.VbaProject;
//Saving the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)



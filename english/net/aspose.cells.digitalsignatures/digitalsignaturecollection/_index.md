---
title: Class DigitalSignatureCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.DigitalSignatures.DigitalSignatureCollection class. Provides a collection of digital signatures attached to a document
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Provides a collection of digital signatures attached to a document.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Constructors

| Name | Description |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | The constructor of DigitalSignatureCollection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Add one signature to DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection |

### Examples

The following example shows how to validate digital signature.

```csharp
[C#]
//workbook from a signed source file
Workbook signedWorkbook = new Workbook(@"signedFile.xlsx");
//wb.IsDigitallySigned is true when the workbook is signed already.
Console.WriteLine(signedWorkbook.IsDigitallySigned);
//get digitalSignature collection from workbook
DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();
foreach (DigitalSignature existingDs in existingDsc)
{
    Console.WriteLine(existingDs.Comments);
    Console.WriteLine(existingDs.SignTime);
    Console.WriteLine(existingDs.IsValid);
}


[Visual Basic]
'workbook from a signed source file
Dim signedWorkbook As Workbook = New Workbook("newfile.xlsx")
'Workbook.IsDigitallySigned is true when the workbook is signed already.
Console.WriteLine(signedWorkbook.IsDigitallySigned)
'get digitalSignature collection from workbook
Dim existingDsc As DigitalSignatureCollection = signedWorkbook.GetDigitalSignature()
Dim existingDs As DigitalSignature
For Each existingDs In existingDsc
    Console.WriteLine(existingDs.Comments)
    Console.WriteLine(existingDs.SignTime)
    Console.WriteLine(existingDs.IsValid)
Next
```

### See Also

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)



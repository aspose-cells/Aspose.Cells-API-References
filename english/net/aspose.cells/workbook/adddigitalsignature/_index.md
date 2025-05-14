---
title: Workbook.AddDigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Adds digital signature to an OOXML spreadsheet file Excel2007 and later
type: docs
url: /net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Remarks

Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file

### Examples

```csharp
// Called: workbook.AddDigitalSignature(digitalSignatureCollection);
public void Workbook_Method_AddDigitalSignature()
{
    string path = Constants.TemplatePath + "NetCoreTests/CELLSNET46964/";

    Workbook workbook = new Workbook(path + "test.xlsx");
    X509Certificate2 certificate =
        new X509Certificate2(path + "DrWatson.pfx", "1234567890");

    //string s1 = certificate.PublicKey.Key.ToXmlString(false);//.NetStandard will crash here

    Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature =
        new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, "Comment", DateTime.Now);

    Aspose.Cells.DigitalSignatures.DigitalSignatureCollection digitalSignatureCollection =
        new Aspose.Cells.DigitalSignatures.DigitalSignatureCollection();

    digitalSignatureCollection.Add(digitalSignature);

    try
    {
        //Exception is here
        workbook.AddDigitalSignature(digitalSignatureCollection);
    }
    catch (Exception ex)
    {
        Console.WriteLine(ex.Message);
    }

    try
    {
        //Exception is here
        workbook.SetDigitalSignature(digitalSignatureCollection);
    }
    catch (Exception ex)
    {
        Console.WriteLine(ex.Message);
    }
    workbook.Save(destPathNetCore + "test_digitally_signed.xlsx");
}
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



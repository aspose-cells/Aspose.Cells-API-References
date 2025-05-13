---
title: Workbook.SetDigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Sets digital signature to an spreadsheet file Excel2007 and later
type: docs
url: /net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Sets digital signature to an spreadsheet file (Excel2007 and later).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Remarks

Only support adding Xmldsig Digital Signature

### Examples

```csharp
// Called: wb.SetDigitalSignature(signs);
public void Workbook_Method_SetDigitalSignature()
{
    string path = Constants.sourcePath + "CELLSNET-46246/";
    Workbook wb = new Workbook(path + "TestCert.xlsx");
    DigitalSignatureCollection signs = new DigitalSignatureCollection();


    DirectoryInfo directoryInfo = new DirectoryInfo(path + "certs");
    FileInfo[] certFiles = directoryInfo.GetFiles();
    foreach (var certFile in certFiles)
    {
        if (certFile.Name.EndsWith(".pfx"))
        {
            //Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature = new Aspose.Cells.DigitalSignatures.DigitalSignature(new System.Security.Cryptography.X509Certificates.X509Certificate2(certFile.FullName, "1234567890"), certFile.Name, DateTime.Now);
            Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature = new Aspose.Cells.DigitalSignatures.DigitalSignature(File.ReadAllBytes(certFile.FullName), "1234567890", certFile.Name, DateTime.Now);
            signs.Add(digitalSignature);
        }
    }
    wb.SetDigitalSignature(signs);

    wb.Save(Constants.destPath + "example.xlsx");

    Console.WriteLine("Start to verify: ");
    Workbook workbook1 = new Workbook(Constants.destPath + "example.xlsx");
    foreach (Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature in workbook1.GetDigitalSignature())
    {
        Assert.IsTrue(digitalSignature.IsValid);
    }
}
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



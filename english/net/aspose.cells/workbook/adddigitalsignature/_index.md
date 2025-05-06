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
[Test]
        public void Method_DigitalSignatureCollection_()
        {
            string path = Constants.TemplatePath + &quot;NetCoreTests/CELLSNET46964/&quot;;

            Workbook workbook = new Workbook(path + &quot;test.xlsx&quot;);
            X509Certificate2 certificate =
                new X509Certificate2(path + &quot;DrWatson.pfx&quot;, &quot;1234567890&quot;);

            //string s1 = certificate.PublicKey.Key.ToXmlString(false);//.NetStandard will crash here

            Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature =
                new Aspose.Cells.DigitalSignatures.DigitalSignature(certificate, &quot;Comment&quot;, DateTime.Now);

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
            workbook.Save(destPathNetCore + &quot;test_digitally_signed.xlsx&quot;);
        }
```

### See Also

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



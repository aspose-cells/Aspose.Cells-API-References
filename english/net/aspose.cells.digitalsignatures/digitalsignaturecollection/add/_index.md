---
title: DigitalSignatureCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignatureCollection method. Add one signature to DigitalSignatureCollection
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/
---
## DigitalSignatureCollection.Add method

Add one signature to DigitalSignatureCollection.

```csharp
public void Add(DigitalSignature digitalSignature)
```

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | Digital signature in collection. |

### Examples

```csharp
// Called: signs.Add(digitalSignature);
[Test]
        public void Method_DigitalSignature_()
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

            wb.Save(Constants.destPath + "CELLSNET-46246_Cs.xlsx");

            Console.WriteLine("Start to verify: ");
            Workbook workbook1 = new Workbook(Constants.destPath + "CELLSNET-46246_Cs.xlsx");
            foreach (Aspose.Cells.DigitalSignatures.DigitalSignature digitalSignature in workbook1.GetDigitalSignature())
            {
                Assert.IsTrue(digitalSignature.IsValid);
            }
        }
```

### See Also

* class [DigitalSignature](../../digitalsignature/)
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)



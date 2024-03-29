---
title: DigitalSignature.DigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature constructor. Constructor of digitalSignature. Uses .Net implementation
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Constructor of digitalSignature. Uses .Net implementation.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| certificate | X509Certificate2 | Certificate object that was used to sign the document. |
| comments | String | The purpose to signature. |
| signTime | DateTime | The utc time when the document was signed. |

### Examples

The following example shows how to create digital signature.

```csharp
[C#]
//signature collection contains one or more signature needed to sign
DigitalSignatureCollection dsc = new DigitalSignatureCollection();
//The cert must contain private key, it can be contructed from cert file or windows certificate collection.
//123456 is password of cert
X509Certificate2 cert = new X509Certificate2("mykey2.pfx", "123456");
DigitalSignature ds = new DigitalSignature(cert, "test for sign", DateTime.Now);
dsc.Add(ds);
Workbook wb = new Workbook();
//set all signatures to workbook
wb.SetDigitalSignature(dsc);
wb.Save(@"newfile.xlsx");


[Visual Basic]
'signature collection contains one or more signature needed to sign
Dim dsc As DigitalSignatureCollection = New DigitalSignatureCollection()
'The cert must contain private key, it can be contructed from cert file or windows certificate collection.
Dim cert As X509Certificate2 = New X509Certificate2("mykey2.pfx", "123456")
'create a signature with certificate, sign purpose and sign time
Dim ds As DigitalSignature = New DigitalSignature(cert, "test for sign", DateTime.Now)
dsc.Add(ds)
Dim wb As Workbook = New Workbook()
'set all signatures to workbook
wb.SetDigitalSignature(dsc)
wb.Save("newfile.xlsx")
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Constructor of digitalSignature. Uses Bouncy Castle implementation.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rawData | Byte[] | A byte array containing data from an X.509 certificate. |
| password | String | The password required to access the X.509 certificate data. |
| comments | String | The purpose to signature. |
| signTime | DateTime | The utc time when the document was signed. |

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)



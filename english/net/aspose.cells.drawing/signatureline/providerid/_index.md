---
title: SignatureLine.ProviderId
second_title: Aspose.Cells for .NET API Reference
description: SignatureLine property. Gets or sets the id of signature provider
type: docs
url: /net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Gets or sets the id of signature provider.

```csharp
public Guid ProviderId { get; set; }
```

### Remarks

It's typically the CLSID of the provider com add-in.

### Examples

```csharp

[C#]
// Create signature line object
SignatureLine s2 = new SignatureLine();
s2.ProviderId = new Guid("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx");//The GUID should be obtained from the documentation shipped with the provider.
```

### See Also

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



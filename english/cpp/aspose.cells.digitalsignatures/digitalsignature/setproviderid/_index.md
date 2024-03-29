﻿---
title: Aspose::Cells::DigitalSignatures::DigitalSignature::SetProviderId method
linktitle: SetProviderId
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DigitalSignatures::DigitalSignature::SetProviderId method. Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells.digitalsignatures/digitalsignature/setproviderid/
---
## DigitalSignature::SetProviderId method


Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.

```cpp
void Aspose::Cells::DigitalSignatures::DigitalSignature::SetProviderId(const UUID &value)
```

## Remarks


The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider. 
## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Typedef [UUID](../../../aspose.cells/uuid/)
* Class [DigitalSignature](../)
* Namespace [Aspose::Cells::DigitalSignatures](../../)
* Library [Aspose.Cells for C++](../../../)

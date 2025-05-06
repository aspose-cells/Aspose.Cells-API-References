---
title: FindOptions.ValueTypeSensitive
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates whether searched cell value type should be same with the searched key
type: docs
url: /net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Indicates whether searched cell value type should be same with the searched key.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Examples

```csharp
// Called: rangeOptions.ValueTypeSensitive = true;
[TestFixtureSetUp]
#endif
        public void Property_ValueTypeSensitive()
        {
            Aspose.Cells.License license = new Aspose.Cells.License();
            license.SetLicense(Constants.licPath);
            options = new FindOptions();
            options.LookAtType = LookAtType.EntireContent;
            options.ValueTypeSensitive = true;
            rangeOptions = new FindOptions();
            rangeOptions.ValueTypeSensitive = true;
            rangeOptions.LookAtType = LookAtType.EntireContent;
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



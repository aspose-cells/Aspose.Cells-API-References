---
title: ExternalConnection.SavePassword
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. True if the password is to be saved as part of the connection string otherwise False
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True if the password is to be saved as part of the connection string; otherwise, False.

```csharp
public bool SavePassword { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.DataConnections[0].SavePassword);
[Test]
        public void Property_SavePassword()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET51696.xls");
            Assert.IsTrue(workbook.DataConnections[0].SavePassword);
            workbook.Save(Constants.destPath + "CELLSNET51696.xlsx");
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)



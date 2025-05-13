---
title: Cell.GetValidationValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the value of validation which applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Gets the value of validation which applied to this cell.

```csharp
public bool GetValidationValue()
```

### Examples

```csharp
// Called: Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
private void Cell_Method_GetValidationValue(Cell cell, char c)
        {
            string sv = c + "";
            cell.PutValue(sv);
            Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
            sv = " " + c;
            cell.PutValue(sv);
            Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
            sv = c + " ";
            cell.PutValue(sv);
            Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
            sv = " " + c + " ";
            cell.PutValue(sv);
            Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
            sv = "     " + c + "   ";
            cell.PutValue(sv);
            Assert.IsTrue(cell.GetValidationValue(), "[" + sv + "]");
            sv = c + "\n";
            cell.PutValue(sv);
            Assert.IsFalse(cell.GetValidationValue(), sv);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



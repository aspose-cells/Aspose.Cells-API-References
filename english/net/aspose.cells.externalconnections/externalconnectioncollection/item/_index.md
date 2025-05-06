---
title: ExternalConnectionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnectionCollection property. Gets the ExternalConnection element at the specified index
type: docs
url: /net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Gets the [`ExternalConnection`](../../externalconnection/) element at the specified index.

```csharp
public ExternalConnection this[int index] { get; set; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: connection = workbook.DataConnections[2];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57031.xlsx&quot;);
            var connection = workbook.DataConnections[0];
            PowerQueryFormula formula = connection.PowerQueryFormula;
            Assert.AreEqual(&quot;end_time&quot;, formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null
            Assert.AreEqual(PowerQueryFormulaType.Parameter, formula.Type);
            Assert.AreEqual(&quot;1543392000&quot;, ((PowerQueryFormulaParameter)formula).Value);

            connection = workbook.DataConnections[1];
            formula = connection.PowerQueryFormula;

            Assert.AreEqual(&quot;fill_url&quot;, formula.Name); // error: null, expected: end_time
            Assert.IsTrue(formula.FormulaDefinition != null); // error: null, expected: not null


            connection = workbook.DataConnections[2];
            formula = connection.PowerQueryFormula;
            Assert.AreEqual(&quot;FIlls&quot;, formula.Name);
            Assert.IsTrue(formula.FormulaDefinition != null);
            workbook.Save(Constants.destPath + &quot;CELLSNET57031.xlsx&quot;);

        }
```

### See Also

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Gets the [`ExternalConnection`](../../externalconnection/) element with the specified name.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parameter | Description |
| --- | --- |
| connectionName | the name of data connection |

### Return Value

The element with the specified name.

### See Also

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)



---
title: Class PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormula class. Represents the definition of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Represents the definition of power query formula.

```csharp
public class PowerQueryFormula
```

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Gets the type of this power query formula. |

### Examples

```csharp
// Called: var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
[Test]
        public void Type_PowerQueryFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet57253.xlsx&quot;);



            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            Assert.AreEqual(&quot;from_timestamp&quot;, powerQueryFormula.Name); // expected: from_timestamp
            Assert.AreEqual(&quot;Fills/t2&quot;, powerQueryFormula.GroupName); // not possible, expected: Other Queries

             powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[1];
            Assert.AreEqual(&quot;start_time&quot;,powerQueryFormula.Name); // expected: start_time
            Assert.AreEqual(&quot;Fills/test&quot;, powerQueryFormula.GroupName); // not possible, expected: Fills / test

            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[2];
            Assert.AreEqual(&quot;limit&quot;, powerQueryFormula.Name); // expected: limit
            Assert.AreEqual(&quot;Fills/test&quot;, powerQueryFormula.GroupName);  // not possible, expected: Fills / test

            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[3];
            Assert.AreEqual(&quot;end_time&quot;, powerQueryFormula.Name); // expected: end_time
            Assert.AreEqual(&quot;Fills/test&quot;, powerQueryFormula.GroupName);   // not possible, expected: Fills / test

            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[4];
            Assert.AreEqual(&quot;FIlls&quot;, powerQueryFormula.Name); // expected: FIlls
            Assert.AreEqual(&quot;Fills/test&quot;, powerQueryFormula.GroupName); // not possible, expected: Fills / test

            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[5];
            Assert.AreEqual(&quot;fill_url&quot;, powerQueryFormula.Name);  // expected: fill_url
            Assert.AreEqual(&quot;Fills/test&quot;, powerQueryFormula.GroupName);// not possible, expected: Fills / test

           


            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[6];
            Assert.AreEqual(&quot;Invoked Function&quot;, powerQueryFormula.Name); // expected: Invoked Function
            Assert.IsTrue(powerQueryFormula.GroupName == null); // not possible, expected: Other Queries

            powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[7];
            Assert.AreEqual(&quot;Table 0&quot;, powerQueryFormula.Name); // expected: Table 0
            Assert.IsTrue(powerQueryFormula.GroupName == null); // not possible, expected: Other Queries
            workbook.Save(Constants.destPath + &quot;CellsNet57253.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)



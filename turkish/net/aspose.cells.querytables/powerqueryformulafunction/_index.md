---
title: "Sınıf PowerQueryFormulaFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaFunction sınıfı. Power query'nin işlevini temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Power Query işlevini temsil eder.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Power query formülünün açıklamasını alır ve ayarlar. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | İşlevin tanımını alır ve ayarlar. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Power query formülünün tanımını alır. ([`PowerQueryFormula`](../powerqueryformula/) üzerinden miras alınmıştır.) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Bu power query formülünü içeren grubun adını alır. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Power query formülünün adını alır ve ayarlar. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Power query formülünün tüm öğelerini alır. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Power query formülünün tipini alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("source.xlsx");
            PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
            
            Console.WriteLine($"Name: {formula.Name}");
            Console.WriteLine($"Type: {formula.Type}");
            
            PowerQueryFormulaFunction function = (PowerQueryFormulaFunction)formula;
            Console.WriteLine($"Signature: {function.F}");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)



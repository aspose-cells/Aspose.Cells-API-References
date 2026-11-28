---
title: "Class PowerQueryFormulaParameter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaParameter sınıfı. Power query formülünün parametresini temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Power Query formülünün parametresini temsil eder.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Power query formülünün açıklamasını alır ve ayarlar. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Parametrenin tanımını alır. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Bu power query formülünü içeren grubun adını alır. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Power query formülünün adını alır ve ayarlar. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Eski.**) Parametrenin tanımını alır. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Power query formülünün tüm öğelerini alır. (Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Power query formülünün tipini alır. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Parametrenin değerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterDemo
    {
        public static void PowerQueryFormulaParameterExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Çalışma kitabının DataMashup özelliğine eriş
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // PowerQueryFormulas özelliğine eriş
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // PowerQueryFormulaParameters özelliğine eriş
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Örnek kullanım: PowerQueryFormulas üzerinden yinele
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Örnek kullanım: PowerQueryFormulaParameters üzerinden yineleyin
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Parametre ayrıntılarını göster
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Çalışma kitabını kaydedin
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)



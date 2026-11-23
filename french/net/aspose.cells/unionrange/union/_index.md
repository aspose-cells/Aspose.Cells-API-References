---
title: "UnionRange.Union"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Fusionne une autre plage"
type: docs
url: /fr/net/aspose.cells/unionrange/union/
---
## Union(string) {#union_2}

Fusionne une autre plage.

```csharp
public UnionRange Union(string range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | String | La plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez la plage initiale et remplissez-la avec des données
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Créez un UnionRange à partir de la plage initiale
            UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            try
            {
                // Appelez la méthode Union avec un paramètre de type chaîne représentant une autre plage
                UnionRange combinedRange = unionRange.Union("C1:D2");

                // Remplissez la deuxième plage avec des données
                worksheet.Cells["C1"].PutValue("Range2");
                worksheet.Cells["D1"].PutValue(300);
                worksheet.Cells["C2"].PutValue("More");
                worksheet.Cells["D2"].PutValue(400);

                Console.WriteLine("Union method executed successfully with parameter (String)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Affichez les informations sur la plage combinée
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(UnionRange) {#union_1}

Fusionne une autre plage.

```csharp
public UnionRange Union(UnionRange unionRange)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | La plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithUnionRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez la première plage et remplissez-la avec des données
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // Créez la deuxième plage et remplissez-la avec des données
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
            range2[0, 0].PutValue("Range2");
            range2[0, 1].PutValue(300);
            range2[1, 0].PutValue("More");
            range2[1, 1].PutValue(400);

            // Créez un UnionRange à partir de la première plage
            UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            // Créez un UnionRange à partir de la deuxième plage
            UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });

            try
            {
                // Appelez la méthode Union avec un paramètre UnionRange
                UnionRange combinedRange = unionRange1.Union(unionRange2);

                Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Affichez les informations sur la plage combinée
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(Range[]) {#union}

Fusionne les plages.

```csharp
public UnionRange Union(Range[] ranges)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plages | Range[] | Les plages. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez des plages d'exemple pour démontrer l'union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Mettez des valeurs dans les plages pour les visualiser
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");
            range3[0, 0].PutValue("Range3");

            try
            {
                // Créez la plage d'union initiale
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Appelez la méthode Union avec un paramètre Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
                UnionRange resultUnion = unionRange.Union(rangesToUnion);

                Console.WriteLine("Union method executed successfully with parameters (Range[])");
                Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
                Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");

                // Mettez en évidence le résultat de l'union en définissant la couleur d'arrière-plan
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
                highlightStyle.Pattern = BackgroundType.Solid;
                resultUnion.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



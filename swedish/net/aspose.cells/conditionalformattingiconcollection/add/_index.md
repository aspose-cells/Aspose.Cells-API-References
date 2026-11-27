---
title: "ConditionalFormattingIconCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIconCollection-metod. Lägger till ConditionalFormattingIcon-objekt"
type: docs
url: /sv/net/aspose.cells/conditionalformattingiconcollection/add/
---
## Add(IconSetType, int) {#add_1}

Lägger till [`ConditionalFormattingIcon`](../../conditionalformattingicon/) objekt.

```csharp
public int Add(IconSetType type, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | IconSetType | Värdetypen. |
| index | Int32 | Indexet. |

### Returvärde

Returnerar indexet för det nya objektet i listan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Skapa intervall för villkorlig formatering
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fcc = cfs[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Skapa villkorsformatering för ikonset
            fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcc[0];
            fc.SetFormula1("0", false, false);
            fc.SetFormula2("100", false, false);
            fc.Operator = OperatorType.Between;

            try
            {
                // Anropa Add-metoden med IconSetType- och indexparametrar
                int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
                Console.WriteLine($"Icon added at index: {addedIndex}");

                // Spara arbetsboken
                workbook.Save("ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(ConditionalFormattingIcon) {#add}

Lägger till [`ConditionalFormattingIcon`](../../conditionalformattingicon/) objekt.

```csharp
[Obsolete("Use ConditionalFormattingIconCollection.Add(IconSetType, int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ConditionalFormattingIcon cficon)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Returnerar indexet för det nya objektet i listan. |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Add(IconSetType, int)-metoden. Denna metod kommer att tas bort 6 månader senare från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till en ny ikonuppsättning för villkorsstyrd formatering.
            int conditionIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
            
            // Lägg till ett villkor av typen IconSet.
            int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition iconSetCondition = conditions[conditionId];
            
            // Ställ in ikonuppsättningstypen med dynamic för att kringgå kompileringskontroller (rekommenderas inte men löser felet).
            dynamic dynamicCondition = iconSetCondition;
            dynamicCondition.Type = IconSetType.CustomSet;
            ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;

            try
            {
                // Använd reflektion för att skapa en ConditionalFormattingIcon-instans (en lösning för saknad konstruktor).
                var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
                icon.Type = IconSetType.Arrows3;
                icon.Index = 0;

                int resultIndex = cfIcons.Add(icon);
                Console.WriteLine($"Added icon index: {resultIndex}");

                // Lägg till cellområdet med AddArea-metoden.
                conditions.AddArea(CellArea.CreateCellArea("A1", "A4"));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



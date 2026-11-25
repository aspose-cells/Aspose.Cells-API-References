---
title: "ConditionalFormattingIconCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConditionalFormattingIconCollection metodo. Aggiunge l'oggetto ConditionalFormattingIcon"
type: docs
url: /it/net/aspose.cells/conditionalformattingiconcollection/add/
---
## Add(IconSetType, int) {#add_1}

Aggiunge [`ConditionalFormattingIcon`](../../conditionalformattingicon/) oggetto.

```csharp
public int Add(IconSetType type, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | IconSetType | Il tipo di valore. |
| indice | Int32 | L'indice. |

### Valore di ritorno

Restituisce l'indice del nuovo oggetto nell'elenco.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Crea intervallo di formattazione condizionale
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fcc = cfs[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Crea formattazione condizionale per il set di icone
            fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcc[0];
            fc.SetFormula1("0", false, false);
            fc.SetFormula2("100", false, false);
            fc.Operator = OperatorType.Between;

            try
            {
                // Chiama il metodo Add con i parametri IconSetType e indice
                int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
                Console.WriteLine($"Icon added at index: {addedIndex}");

                // Salva la cartella di lavoro
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

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(ConditionalFormattingIcon) {#add}

Aggiunge [`ConditionalFormattingIcon`](../../conditionalformattingicon/) oggetto.

```csharp
[Obsolete("Use ConditionalFormattingIconCollection.Add(IconSetType, int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ConditionalFormattingIcon cficon)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Restituisce l'indice del nuovo oggetto nell'elenco. |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Add(IconSetType, int). Questo metodo sarà rimosso 6 mesi dopo, a partire da dicembre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

            // Aggiungi una nuova formattazione condizionale di set di icone
            int conditionIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
            
            // Aggiungi una condizione di tipo IconSet
            int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition iconSetCondition = conditions[conditionId];
            
            // Imposta il tipo di set di icone usando dynamic per aggirare i controlli a tempo di compilazione (non consigliato ma risolve l'errore)
            dynamic dynamicCondition = iconSetCondition;
            dynamicCondition.Type = IconSetType.CustomSet;
            ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;

            try
            {
                // Utilizzando la riflessione per creare un'istanza di ConditionalFormattingIcon (soluzione alternativa per costruttore mancante)
                var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
                icon.Type = IconSetType.Arrows3;
                icon.Index = 0;

                int resultIndex = cfIcons.Add(icon);
                Console.WriteLine($"Added icon index: {resultIndex}");

                // Aggiungi l'area della cella usando il metodo AddArea
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

### Vedi anche

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadFilter-Eigenschaft. Gibt die Blattindizes und die Reihenfolge an, die geladen werden sollen. Standard ist null, was bedeutet, dass alle Blätter in der Standardreihenfolge der Vorlagendatei geladen werden. Wenn nicht null und ein Blattindex nicht im zurückgegebenen Array enthalten ist, wird das Blatt nicht geladen."
type: docs
url: /de/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Gibt die zu ladenden Blätter (Indizes) und deren Reihenfolge an. Standard ist null, was bedeutet, dass alle Blätter in der Standardreihenfolge der Vorlagendatei geladen werden. Wenn nicht null und ein Blattindex nicht im zurückgegebenen Array enthalten ist, wird dieses Blatt nicht geladen.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit mehreren Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Erstellen Sie einen benutzerdefinierten Ladefilter
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Zeigen Sie die Standard-SheetsInLoadingOrder an (null bedeutet, alle Blätter zu laden)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Erstellen Sie eine Vorlagendatei, um das Laden mit benutzerdefinierter Blattreihenfolge zu demonstrieren
            workbook.Save("Template.xlsx");
            
            // Erstellen Sie Ladeoptionen mit unserem benutzerdefinierten Filter
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Laden Sie die Arbeitsmappe mit den Standardeinstellungen (alle Blätter)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Erstellen Sie einen neuen Filter mit einer spezifischen Blattlade-Reihenfolge
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Hinweis: SheetsInLoadingOrder ist schreibgeschützt, daher müssen wir einen neuen Filter erstellen
                // mit der gewünschten Reihenfolge im Konstruktor oder auf andere Weise
                // Dies demonstriert die Einschränkung, dass die Eigenschaft schreibgeschützt ist
            };
            
            // Da SheetsInLoadingOrder schreibgeschützt ist, müssen wir LoadFilter unterklassen
            // um die benutzerdefinierte Blattlade-Reihenfolge zu demonstrieren
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Arbeitsmappe mit benutzerdefinierter Blattreihenfolge laden
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Benutzerdefinierte LoadFilter-Implementierung, um die Funktionalität von SheetsInLoadingOrder zu demonstrieren
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### Siehe auch

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



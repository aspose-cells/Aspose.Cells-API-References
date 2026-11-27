---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadFilter‑egenskap. Anger bladindex och ordning som ska laddas. Standard är null vilket betyder att alla blad laddas i standardordning i mallfilen. Om den inte är null och ett bladindex saknas i den returnerade arrayen kommer bladet inte att laddas"
type: docs
url: /sv/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Anger vilka blad (index) och i vilken ordning de ska läsas in. Standard är null, vilket betyder att alla blad läses in i standardordning i mallfilen. Om värdet inte är null och ett bladindex inte finns i den returnerade arrayen, kommer bladet inte att läsas in.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Skapa ett anpassat laddningsfilter
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Visa standardvärdet för SheetsInLoadingOrder (null betyder att alla blad laddas)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Skapa en mallfil för att demonstrera laddning med anpassad bladordning
            workbook.Save("Template.xlsx");
            
            // Skapa laddningsalternativ med vårt anpassade filter
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Ladda arbetsboken med standardinställningar (alla blad)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Skapa ett nytt filter med specifik bladladdningsordning
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Obs: SheetsInLoadingOrder är skrivskyddad, så vi måste skapa ett nytt filter
                // med önskad ordning i konstruktorn eller på annat sätt
                // Detta demonstrerar begränsningen av att egenskapen är skrivskyddad
            };
            
            // Eftersom SheetsInLoadingOrder är skrivskyddad måste vi subklassa LoadFilter
            // för att demonstrera anpassad bladladdningsordning
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Läs in arbetsbok med anpassad bladordning
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Anpassad LoadFilter-implementation för att demonstrera funktionaliteten i SheetsInLoadingOrder
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

### Se även

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "PivotField.GroupBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Grupperar automatiskt fältet med intervall"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Gruppera automatiskt fältet med intervall

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intervall | Double | Den interna för gruppen. Automatiskt värde kommer att tilldelas om det är noll, |
| newField | Boolean | Anger om ett nytt fält läggs till i pivottabellen. Endast för DateTime-grupp. |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Lägg till fält i kolumnområdet
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Gruppera fältet med 1 (intervall) med automatiskt intervall
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Gruppera automatiskt fältet med intern

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| grupper | PivotGroupByType[] | Grupptyper |
| intervall | Double | Den interna delen av gruppen. Automatiskt värde kommer att tilldelas om det är noll, fungerar endast för gruppering efter nummer eller dagar. |
| newField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen. |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Gruppera filen efter datumgruppningstyper.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | DateTime | Startdatum och tid |
| slut | DateTime | Slutdatum och tid |
| grupper | PivotGroupByType[] | Grupptyper |
| intervall | Double | Intervallet |
| firstAsNewField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen. Endast för det första gruppobjektet. |

### Returvärde

Falskt betyder att detta fält inte kan grupperas efter datum och tid.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med datum för pivottabellen
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            // Förbered parametrar för GroupBy-metoden
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Anropa GroupBy-metoden med datumparametrar
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Uppdatera pivottabell
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Gruppera filen efter datumgruppningstyper.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoStart | Boolean | Anger om startdatum- och tidsvärdet ska upptäckas automatiskt. |
| start | DateTime | Startdatum och tid |
| isAutoEnd | Boolean | Anger om slutdatum- och tidsvärdet ska upptäckas automatiskt. |
| slut | DateTime | Slutdatum och tid |
| grupper | PivotGroupByType[] | Grupptyper |
| intervall | Double | Intervallet |
| firstAsNewField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen. Endast för det första gruppobjektet. |

### Returvärde

Falskt betyder att detta fält inte kan grupperas efter datum och tid.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Gruppera filen efter nummer.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | Double | Startvärdet |
| slut | Double | Slutvärdet |
| intervall | Double | Intervallet |
| newField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen |

### Returvärde

Falskt betyder att detta fält inte kan grupperas efter datum och tid.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och gruppera det
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Spara arbetsboken
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Gruppera filen efter nummer.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoStart | Boolean | Anger om startvärdet ska upptäckas automatiskt. |
| start | Double | Startvärdet |
| isAutoEnd | Boolean | Anger om slutvärdet ska upptäckas automatiskt. |
| slut | Double | Slutvärdet |
| intervall | Double | Intervallet |
| newField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen |

### Returvärde

Falskt betyder att detta fält inte kan grupperas efter datum och tid.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions) metod. Denna metod kommer att tas bort 6 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Anpassa gruppering av fältet.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | De anpassade gruppobjekten. |
| newField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen |

### Returvärde

Falskt betyder att detta fält inte kan grupperas efter datum och tid.

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions options)-metoden med PivotFieldGroupOptions.DiscreteGroupItems-egenskapen. Denna metod kommer att tas bort 6 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            // Skapa anpassade gruppobjekt
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Anropa GroupBy-metoden med anpassade gruppobjekt
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Uppdatera pivottabell
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Anpassa gruppering av fältet.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | De anpassade gruppobjekten. |
| newField | Boolean | Anger om ett nytt fält ska läggas till i pivottabellen |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotField.Group(PivotFieldGroupOptions options)-metoden med PivotFieldGroupOptions.DiscreteGroupItems-egenskapen. Denna metod kommer att tas bort 6 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



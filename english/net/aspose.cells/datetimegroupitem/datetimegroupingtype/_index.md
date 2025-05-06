---
title: DateTimeGroupItem.DateTimeGroupingType
second_title: Aspose.Cells for .NET API Reference
description: DateTimeGroupItem property. Gets and sets the group type
type: docs
url: /net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Gets and sets the group type.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Modified DateTimeGroupingType: &amp;quot; + dateTimeGroupItem.DateTimeGroupingType);
public static void Property_DateTimeGroupingType()
        {
            // Create an instance of DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Accessing properties
            Console.WriteLine(&quot;MinValue: &quot; + dateTimeGroupItem.MinValue);
            Console.WriteLine(&quot;DateTimeGroupingType: &quot; + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine(&quot;Year: &quot; + dateTimeGroupItem.Year);
            Console.WriteLine(&quot;Month: &quot; + dateTimeGroupItem.Month);
            Console.WriteLine(&quot;Day: &quot; + dateTimeGroupItem.Day);
            Console.WriteLine(&quot;Hour: &quot; + dateTimeGroupItem.Hour);
            Console.WriteLine(&quot;Minute: &quot; + dateTimeGroupItem.Minute);
            Console.WriteLine(&quot;Second: &quot; + dateTimeGroupItem.Second);

            // Modifying properties
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Accessing modified properties
            Console.WriteLine(&quot;Modified DateTimeGroupingType: &quot; + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine(&quot;Modified Year: &quot; + dateTimeGroupItem.Year);
            Console.WriteLine(&quot;Modified Month: &quot; + dateTimeGroupItem.Month);
            Console.WriteLine(&quot;Modified Day: &quot; + dateTimeGroupItem.Day);
            Console.WriteLine(&quot;Modified Hour: &quot; + dateTimeGroupItem.Hour);
            Console.WriteLine(&quot;Modified Minute: &quot; + dateTimeGroupItem.Minute);
            Console.WriteLine(&quot;Modified Second: &quot; + dateTimeGroupItem.Second);
        }
```

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: Cells.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the memory usage option for this cells
type: docs
url: /net/aspose.cells/cells/memorysetting/
---
## Cells.MemorySetting property

Gets or sets the memory usage option for this cells.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: cells.MemorySetting = MemorySetting.Normal;
internal void Cells_Property_MemorySetting()
            {
                Console.WriteLine("Testing MultiThreadReading for Normal model...");
                cells.MemorySetting = MemorySetting.Normal;
                Thread myThread1 = new Thread(new ThreadStart(ThreadLoop));
                Thread myThread2 = new Thread(new ThreadStart(ThreadLoop));

                myThread1.Start();
                myThread2.Start();
                myThread1.Join();
                myThread2.Join();
                Console.WriteLine("Finished.");

                Console.WriteLine("Testing MultiThreadReading for Memory model...");
                cells.MemorySetting = MemorySetting.MemoryPreference;
                myThread1 = new Thread(new ThreadStart(ThreadLoop));
                myThread2 = new Thread(new ThreadStart(ThreadLoop));
                myThread1.Start();
                myThread2.Start();
                myThread1.Join();
                myThread2.Join();
                Console.WriteLine("Finished.");
            }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



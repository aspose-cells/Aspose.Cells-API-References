---
title: AbstractInterruptMonitor
second_title: Aspose.Cells for .NET API Referansı
description: Tüm zaman alan işlemlerde kesinti isteklerini izleyin.
type: docs
weight: 50
url: /tr/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Tüm zaman alan işlemlerde kesinti isteklerini izleyin.

```csharp
public abstract class AbstractInterruptMonitor
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested) { get; } | Mevcut işlem için kesinti istenip istenmediğini gösterir. Doğruysa mevcut işlem kesintiye uğrayacaktır. Uygulama burada hızlı ve verimli bir kontrol gerçekleştirmelidir, aksi takdirde prosedür için başka bir darboğaz haline gelebilir. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception) { get; } | Prosedür kesintiye uğradığında, prosedürü sessizce sonlandırın veya bir İstisna atın. Varsayılan yanlıştır, yani[`IsInterruptionRequested`](./isinterruptionrequested) doğrudur, bir[`CellsException`](../cellsexception) kodluInterrupted atılacak. |

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
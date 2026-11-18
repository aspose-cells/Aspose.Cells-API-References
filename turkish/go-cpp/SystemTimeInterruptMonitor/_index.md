---
title: "SystemTimeInterruptMonitor Class"
linktitle: "SystemTimeInterruptMonitor"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SystemTimeInterruptMonitor class. Go dilinde systemtimeinterruptmonitor'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Mevcut sistem zamanını kullanıcı tarafından belirtilen limit ile kontrol edip karşılaştırarak <see cref="AbstractInterruptMonitor"/>'nin basit bir uygulaması.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Bir kesinti izleyicisi oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [StartMonitor](./startmonitor/) | İzleyiciyi belirtilen zaman sınırıyla başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı an olur, bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Bu uygulama, zaman maliyetinin (izleyicinin başlatıldığı andan şimdiki zamana kadar) kullanıcı tarafından belirtilen sınırdan büyük olup olmadığını sadece kontrol eder. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | AbstractInterruptMonitor.TerminateWithoutException'a bakın. Bu özellik, bu izleyici örneği oluşturulurken kullanıcı tarafından belirtilir. |

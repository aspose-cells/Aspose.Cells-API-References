##Metered.SetMeteredKey
Metered method. Sets metered public and private key. If you purchase metered license when start application this API should be called normally this is enough. However if always fail to upload consumption data and exceed 24 hours the license will be set to evaluation status to avoid such case you should regularly check the license status if it is evaluation status call this API again
## Metered.SetMeteredKey method
Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.
```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MeteredMethodSetMeteredKeyWithStringStringDemo
{
public static void Run()
{
// Set metered public and private keys
Metered metered = new Metered();
metered.SetMeteredKey(
"asposenet7c90badb00ba4f4bbd35634f4d481c14",
"FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");
// Get metered consumption quantity
decimal consumption = Metered.GetConsumptionQuantity();
Console.WriteLine("Consumption quantity: " + consumption);
// Get metered consumption credit
decimal credit = Metered.GetConsumptionCredit();
Console.WriteLine("Consumption credit: " + credit);
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

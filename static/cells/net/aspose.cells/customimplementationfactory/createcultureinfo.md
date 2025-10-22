##CustomImplementationFactory.CreateCultureInfo
CustomImplementationFactory method. Create one CultureInfo by given id
## CustomImplementationFactory.CreateCultureInfo method
Create one CultureInfo by given id.
```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```
| Parameter | Type | Description |
| --- | --- | --- |
| lcid | Int32 |  |
### Return Value
The CultureInfo instance.
### Remarks
This implementation is useful for situations: 1. Some cultures may not be supported by user's environment and creating the required CultureInfo with given identifier may cause Exception. To avoid the exception, user may override this method to provide a valid CultureInfo instance for the unsupported one. 2. User may want to specify some custom properties for some cultures to get expected result for formatting. For this purpose user may override this method to provide the CultureInfo instance with user specified properties. Please note UseUserOverride property of the returned CultureInfo instance may influence the formatted result. If it is false, some properties of the returned CultureInfo instance may be overridden by our built-in formatting engine according to the formatting requirements of different scenarios. If it is true, we will not change any properties of it and use it to format values directly. So, if user has specified custom properties for the returned CultureInfo instance, please make sure its UseUserOverride is true.
### See Also
* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

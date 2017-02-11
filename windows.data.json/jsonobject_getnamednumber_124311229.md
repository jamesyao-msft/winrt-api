---
-api-id: M:Windows.Data.Json.JsonObject.GetNamedNumber(System.String,System.Double)
-api-type: winrt method
---

<!-- Method syntax
public double GetNamedNumber(System.String name, System.Double defaultValue)
-->

# Windows.Data.Json.JsonObject.GetNamedNumber

## -description
Gets the number value (a [Double](https://msdn.microsoft.com/library/system.double.aspx)) with the specified name, or the provided default value if no such named value is found.

## -parameters
### -param name
The name.

### -param defaultValue
The default value to use if the JSON property is not found.

## -returns
The [Double](https://msdn.microsoft.com/library/system.double.aspx) with the specified *name*, or if this value wasn't found, the *defaultValue* is returned.

## -remarks
This method should always used with a try/catch block because it throws an exception if the name is not found.

## -examples

## -see-also
[GetNamedNumber(String)](jsonobject_getnamednumber_448999001.md)
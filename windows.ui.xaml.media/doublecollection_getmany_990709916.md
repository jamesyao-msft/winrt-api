---
-api-id: M:Windows.UI.Xaml.Media.DoubleCollection.GetMany(System.UInt32,System.Double[])
-api-type: winrt method
---

<!-- Method syntax
public uint GetMany(System.UInt32 startIndex, System.Double[] items)
-->

# Windows.UI.Xaml.Media.DoubleCollection.GetMany

## -description
Retrieves multiple elements in a single pass through the iterator.

## -parameters
### -param startIndex
The index from which to start retrieval.

### -param items
Provides the destination for the result. Size the initial array size as a "capacity" in order to specify how many results should be retrieved.

## -returns
The number of items retrieved.

## -remarks
The [GetMany](doublecollection_getmany.md) method operates identically as if calling  and  for each element in the supplied array. This means that the first element returned by the [GetMany](doublecollection_getmany.md) method is the same element as returned by retrieving the  property prior to calling [GetMany](doublecollection_getmany.md). After the [GetMany](doublecollection_getmany.md) call returns, the  property will retrieve the element following the last element returned by the [GetMany](doublecollection_getmany.md) call, or produce an error if no more elements exist in the sequences.

The [GetMany](doublecollection_getmany.md) method returns the actual number of elements returned. It must be the minimum of a) the number of elements remaining in the collection, or b) the number of elements requested, that is "capacity". Therefore, whenever [GetMany](doublecollection_getmany.md) returns fewer than the number of elements requested, the end of the sequence has been reached. It returns the number of elements retrieved in the "actual" output parameter.

When the caller specifies a capacity of zero, the position of the iterator is unchanged. Elements in the array following the values returned are unchanged.

## -examples

## -see-also
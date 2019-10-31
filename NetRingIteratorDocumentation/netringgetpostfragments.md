# NetRingGetPostFragments method


## Description



The **NetRingGetPostFragments** method gets a fragment iterator for the current post subsection of a fragment ring.

## Syntax

```C++
NET_RING_FRAGMENT_ITERATOR NetRingGetPostFragments(
  NET_RING_COLLECTION const *Rings
);
```

## Parameters

### Rings

A pointer to the [**NET_RING_COLLECTION**](https://docs.microsoft.com/windows-hardware/drivers/ddi/ringcollection/ns-ringcollection-_net_ring_collection) struture that describes the packet queue's net rings.

## Returns

Returns a [**NET_RING_FRAGMENT_ITERATOR**](net_ring_fragment_iterator.md) that begins at the fragment ring's **NextIndex** and ends at the fragment ring's **EndIndex**. In other words, the iterator covers the fragment ring's current post subsection.

## Remarks

Client drivers typically call **NetRingGetPostFragments** to begin the process of posting fragments to hardware for receiving (Rx). Drivers later complete this process by calling [**NetFragmentIteratorSet**](netfragmentiteratorset.md).

For a code example of posting fragments to hardware for Rx, see the [Net ring iterator README](README.md).

## Requirements

| | |
| --- | --- |
| Header | netringiterator.h |
| IRQL | Any level as long as target memory is resident |

## See Also

[Net ring iterator README](README.md)

[**NET_RING_COLLECTION**](https://docs.microsoft.com/windows-hardware/drivers/ddi/ringcollection/ns-ringcollection-_net_ring_collection)

[**NET_RING_FRAGMENT_ITERATOR**](net_ring_fragment_iterator.md)

[**NetFragmentIteratorSet**](netfragmentiteratorset.md)

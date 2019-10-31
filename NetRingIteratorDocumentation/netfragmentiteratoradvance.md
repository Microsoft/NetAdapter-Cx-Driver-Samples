# NetFragmentIteratorAdvance method


## Description



The **NetFragmentIteratorAdvance** method advances the Index of a fragment iterator by one.

## Parameters

### Iterator

A pointer to a [**NET_RING_FRAGMENT_ITERATOR**](net_ring_fragment_iterator.md) structure.

## Returns

None.

## Remarks

If the fragment iterator's current **Index** is at the end of the fragment ring, this method automatically handles wrapping around to the beginning of the ring.

## See Also

[Net ring iterator README](readme.md)

[**NET_RING_FRAGMENT_ITERATOR**](net_ring_fragment_iterator.md)
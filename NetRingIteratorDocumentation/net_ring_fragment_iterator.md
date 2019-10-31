# NET_RING_FRAGMENT_ITERATOR structure

## Description



A **NET_RING_FRAGMENT_ITERATOR** is a wrapper around a [**NET_RING_ITERATOR**](net_ring_iterator.md) that client drivers use for net fragment rings.

## -struct-fields

### -field Iterator

The [**NET_RING_ITERATOR**](net_ring_iterator.md) structure around which this structure wraps. 

## -remarks

For fragment rings, client drivers must use a **NET_RING_FRAGMENT_ITERATOR** instead of using a [**NET_RING_ITERATOR**](net_ring_iterator.md) directly.

## See Also

[Net ring iterator README](readme.md)

[**NET_RING_ITERATOR**](net_ring_iterator.md)
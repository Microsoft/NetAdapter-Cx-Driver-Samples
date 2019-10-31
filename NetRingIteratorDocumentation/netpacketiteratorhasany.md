# NetPacketIteratorHasAny method


## Description



The **NetPacketIteratorHasAny** method determines whether a packet iterator has any valid elements to process in the packet ring.

## Parameters

### Iterator

A pointer to a [**NET_RING_PACKET_ITERATOR**](net_ring_packet_iterator.md) structure.

## Returns

Returns **TRUE** if the iterator's **Index** does not equal its **End** index. In other words, the iterator has a packet to process. Otherwise, returns **FALSE**.

## Remarks

Client drivers can call **NetPacketIteratorHasAny** to test if the iterator has any valid elements to process. This method can be used to verify a packet before processing it, or it can be used as a test condition for a loop when the driver is processing multiple packets in a batch.

## See Also

[Net ring iterator README](readme.md)

[**NET_RING_PACKET_ITERATOR**](net_ring_packet_iterator.md)

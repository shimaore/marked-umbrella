marked-umbrella is a process running on a CCNQ4 backend (VoIP or other)

It interfaces
- with other local processes using a Redis pub/sub instance (via `red-rings-redis/backend`)
- with upstream/other red-rings processes (especially abrasive-ducks) using Axon.

Other local processes connect the Redis pub/sub using `red-rings-redis`.

Since we do not have an architecure for Axon discovery yet, the remote Axon nodes are currently statically configured.

# D.A.F.A.R.T Proof of Concept


## Summary
A proof of concept is no good without a concept to prove. This proof of concept hopes to show that we can establish a reliable connection between 2 end points seperated by an obstruction that denies a direct physical link via the usage of one intermedary relay node. 


## Objective 
Prove that mesh network topology can relibably transmited data between two non line of sight endpoints using a single relay node.


## Success Criteria

- Mimimum throughput: 15 Mbps Sustained, reflects real world conditions
- Latency: < 100ms, reflects close to real time constraints
- Packet Loss: <1%, relfects reliatbility requirements
- Use Case Validation: video streaming, ROS2 for extra points, relfects real use case.


## Test Architecture

- Node A: Raspberry PI with OpenWRT (connected to destination computer via Ethernet)
- Node B: Raspberry PI with OpenWRT (standalone mesh relay)
- Node C: Raspberry PI with OpenWRT (source, providing video)

### Network Topology
The network topology below presents what an implmentation of a mesh network would look like with the star being the B.A.T.M.A.N. Advanced interface on layer 2. An acompanying bridge interface is also present to provide an interface to ethernet devices to access the networks resources. 

<img width="2604" height="1764" alt="image" src="https://github.com/user-attachments/assets/6a45d6e9-0381-4777-9833-d590b80a2482" />

### Test Plan

Start with a point to point connection over mesh.

**Add one node**

Make connection A -> C really bad, while keeping A <-> B and B <-> C good.
Verify that A <-> B <-> C is prioritized and network quality is preserved.

Isolate and kill direct connection between A <-> C
Verify connection still exists via A <-> B <-> C

Make connection A <-> B <-> C really bad, while keeping A <-> C good.
Verify that A <-> C is prioritized and network quality is preserved.


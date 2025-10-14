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



### Physical Topology

# Routing performance evaluation tests

To evaluation maximum performance capability of TheRouter number of test was conducted.
Performed tests try to cover all dirrent types of traffic and load that a router can face
in a real network. To generate different traffic types a PktGen software was used. PktGen
is DPDK based stateless packet generator capable of creation traffic with different parameters
practically on wire speed. Main traffic parameters that was covered by tests are:
 - pps - packet per second
 - packet size
 - number of ip flows

Also different TheRouter configurations was tested that were differed by:
 - number of routes
 - port configuration

Also several different network schemes was tested such as:
 - unidirection traffic tests
 - bidirection traffic tests
 - 4-directional traffic tests
 - 4-directional LACP tests

### Unidirection and bidirectional test lab schemes
<img src="http://therouter.net/images/tests/routing_tests/27_01_2018/ub_tests.png">

### 4-direction test lab schemes
<img src="http://therouter.net/images/tests/routing_tests/27_01_2018/4dir_tests.png">

Results:
Test have showed that TheRouter is capable of forwarding up to 32Mpps 64 bytes packets with 0 packet loss 
(test 14.3 in the table with full results below). 

In more complicated test scenario when router was configured with LACP bonding port and 800k routes were installed into
its FIB it showed result of 20 Mpps with zero packet loss.

# Full results table:
 - <a href="http://therouter.net/images/tests/routing_tests/27_01_2018/router_test_21.01.2018_routing_test1_wo_borders.html">html table</a>
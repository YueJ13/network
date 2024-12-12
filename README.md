# multistability

To prove if the network G only admits degenerate positive steady states, then G does not admit finite positive steady states, the readers can use the files in the path “multistability/degenerate”. 
The readers can run “check_finite.mw” (need “jach=0_f.xlsx”) in Maple to check whether the networks admit finite positive steady states. The file “jach=0_f.xlsx” is the result of running “find_J=0.nb” in Mathematica and enumerates the steady-state system of the networks only admitting degenerate positive steady states.
To check the sign of determinant of Jacobian matrix of system h of all two-dimensional three-species subnetworks of the networks in g_2 and g_3, the readers can use the files in the path “multistability/jach_positive”. 
The readers can run “check_subnetwork_Jach.nb” in Mathemetica. Note that the readers need to install R. To see the detail of the algorithm, the readers can run “detailed_check_jach.nb” in Mathemetica, which displays every step of algorithm by an example. 

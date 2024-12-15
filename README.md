# multistability
# Here, we provide the codes and data associated with the preprint: "Multistability of Small Zero-One Reaction Networks" (https://arxiv.org/abs/2208.04196), written by Yue Jiao, Xiaoxian Tang and Xiaowei Zeng.

# 1.
# To find all three-species five-reaction zero-onetworks which admit multistationarity/ multistability, the readers can use the files under the path "multistability/smallest".

# First, The readers can run "delete_injective_networks.nb" (need "s3r5_01_tri_rank3_ND.simp.cpp") in Mathematica to delete the injective networks. The result is directly demonstrated in "odesystem.xls", in which are the steady-state systems of 39233 networks.

# Second, the readers can run "check_more_3_steady_states.mw" (need "odesystem.xls") in Maple to check whether the networks admit more than three positive steady states. The result is directly demonstrated in "results_of_check_more_than_3--1.xlsx" and "results_of_check_more_than_3--2.xlsx".

# Then, the readers can run "check_2_steady_states.mw" (need "odesystem.xls") in Maple to check whether the networks admit two positive steady states. The result is directly demonstrated in "results_of_check_2--1.xlsx" and "results_of_check_2--2.xlsx". There are 252 networks admitting tow positive steady states. (If the result of a network is empty or "Warning", the readers can check the steady states of the network by "empty_warning.mw".)

# Last, the readers can use "check_sgn.mw" in Maple to check the sign of the determinant of Jacobian matrix of system h evaluating in two positive steady states. ("Part 1" is used to check the multistability of the networks which results are not empty or "Warning". "Part 2" is used to check the multistability of the networks which results are empty or "Warning".)

# 2.
# To prove if the network G only admits degenerate positive steady states, then G does not admit finite positive steady states, the readers can use the files under the path "multistability/degenerate". 

# The readers can run "check_finite.mw" (need "jach=0_f.xlsx") in Maple to check whether the networks admit finite positive steady states. The file "jach=0_f.xlsx" is the result of running "find_J=0.nb" in Mathematica and enumerates the steady-state systems of the networks only admitting degenerate positive steady states.

# 3.
# To check the sign of the determinant of Jacobian matrix of system h of all two-dimensional three-species subnetworks of the networks in g_2 and g_3, the readers can use the files under the path "multistability/jach_positive". 

# The readers can run "check_subnetwork_Jach.nb" in Mathemetica. To see the detail of the algorithm, the readers can run "detailed_check_jach.nb" in Mathemetica, which displays every step of algorithm by an example. 

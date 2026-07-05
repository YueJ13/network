# Multistability of Small Zero-One Reaction Networks

This repository contains the code and data accompanying the paper:

**["Multistability of Small Zero-One Reaction Networks"](https://doi.org/10.1007/s00285-025-02306-w)**  
by Yue Jiao, Xiaoxian Tang, and Xiaowei Zeng.

---

## Part 1: Finding Three-Species Five-Reaction Zero-One Networks with Multistationarity/Multistability

To find all three-species five-reaction zero-one networks that admit multistationarity or multistability, use the files under the path:

`multistability/smallest`

### Step 1: Delete Injective Networks

Run **`delete_injective_networks.nb`** in Mathematica (requires `s3r5_01_tri_rank3_ND.simp.cpp`).

This deletes the injective networks. The result is directly demonstrated in **`odesystem.xls`**, which contains the steady-state systems of 39,233 networks.

### Step 2: Check for More Than Three Positive Steady States

Run **`check_more_3_steady_states.mw`** in Maple (requires `odesystem.xls`).

This checks whether the networks admit more than three positive steady states. The results are directly demonstrated in:
- `results_of_check_more_than_3--1.xlsx`
- `results_of_check_more_than_3--2.xlsx`

### Step 3: Check for Two Positive Steady States

Run **`check_2_steady_states.mw`** in Maple (requires `odesystem.xls`).

This checks whether the networks admit two positive steady states. The results are directly demonstrated in:
- `results_of_check_2--1.xlsx`
- `results_of_check_2--2.xlsx`

**Note:** There are 429 networks admitting two positive steady states. If the result of a network is empty or shows "Warning", you can check the steady states of that network using **`empty_warning.mw`**.

### Step 4: Check Sign of Jacobian Determinant

Run **`check_sgn.mw`** in Maple to check the sign of the determinant of the Jacobian matrix of system *h* evaluated at two positive steady states.

- **Part 1:** Used to check the multistability of networks whose results are not empty or do not show "Warning".
- **Part 2:** Used to check the multistability of networks whose results are empty or show "Warning".

---

## Part 2: Degenerate Positive Steady States

To prove that if network *G* only admits degenerate positive steady states, then *G* does not admit finite positive steady states, use the files under the path:

`multistability/degenerate`

### Check for Finite Positive Steady States

Run **`check_finite.mw`** in Maple (requires `jach=0_f.xlsx`).

This checks whether the networks admit finite positive steady states. The file **`jach=0_f.xlsx`** is the result of running **`find_J=0.nb`** in Mathematica and enumerates the steady-state systems of the networks that only admit degenerate positive steady states.

---

## Part 3: Checking Jacobian Determinant of Subnetworks

To check the sign of the determinant of the Jacobian matrix of system *h* for all two-dimensional three-species subnetworks of the networks in *g_2* and *g_3*, use the files under the path:

`multistability/jach_positive`

### Run the Main Check

Run **`check_subnetwork_Jach.nb`** in Mathematica.

### View Detailed Algorithm

To see the details of the algorithm, run **`detailed_check_jach.nb`** in Mathematica. This displays every step of the algorithm using an example.

---

# JAX-MD-atomic-bond-length-distances-VASP
Calculate the bond length between specific atoms from the XDATCAR during VASP molecular dynamics calculations.

It outputs the value only of those bonds below a specified threshold.

This code bond_original2.py is meant for NpT calculation where the volume is varying at every step of the MD.

Line 62 is telling the code to calculate the distances between atome 64 till last one.

mat = np.linalg.norm(distance_matrix(pos[64:],pos[64:]), axis=-1)

You can change this at your own need.

Bond-nvt-nve.py solves analogous task at fixed volume.

# JAX-MD-atomic-bond-length-distances-VASP
Calculate the bond length between specific atoms from the XDATCAR during VASP molecular dynamics calculations.

It outputs the value only of those bonds below a specified threshold.

This code is meant for NpT calculation where the volume is varying at every step of the MD, if you run NvT you should adapt it to your case and should be easier.

Line 62 is telling the code to calculate the distances between atome 64 till last one.

mat = np.linalg.norm(distance_matrix(pos[64:],pos[64:]), axis=-1)

You can change this at your own need.

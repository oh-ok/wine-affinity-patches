## Wine/Affinity Patches

I made these for personal uses, since I was sick of how slow CPU only compute was on Affinity, so don't expect anything incredible!

### dxcore.patch
An implemetation of the IDXCoreAdapterFactory, IDXCoreAdapterList and IDXCoreAdapter interfaces.

### opencl.patch
Advertises the `cl_khr_d3d10_sharing` extension to the host app.

As far as I can tell, the Affinity programs check for, but never actually _use_ the `cl_khr_d3d10_sharing` extension to share data, only to query available devices. Maybe in a specific usecase it will, though. If I get really bored, I may try to replicate the entire `*_sharing` extension suite if I can figure out how they work.

### wintypes.patch
A slightly more "correct" (but more complex) version of ElementalWarriors RoResolveNamespace patch.

#### Electrostatics静电学
coulombtype = Cut-off ；Plain cut-off with neighborlist radius rlist and Coulomb cut-off rcoulomb, where rlist >= rcoulomb 用邻近列表半径和库伦截断半径的简单的截断，其中rlist大于等于rcoulomb

coulombtype = Ewald ; Classical Ewald sum electrostatics. The real-space cut-off rcoulomb should be equal to rlist. Use e.g. rlist =0.9, rcoulomb =0.9. The highest magnitude of wave vectors used in reciprocal space is controlled by fourierspacing. The relative accuracy of direct/reciprocal space is controlled by ewald-rtol.NOTE: Ewald scales as O(N^3/2) and is thus extremely slow for large systems. It is included mainly for reference - in most cases PME will perform much better.经典Ewald合计静电学。真空间截断rcoulomb应该等于rlist。比如，rlist=0.9, rcoulomb=0.9。倒空间中，波矢量的最高的数量是由fourierspacing傅里叶间距控制的。直接或者倒空间的相对精度由ewald-rtol控制。注释：对于大体系，Ewald scales 作为O(N^3/2)因此是非常慢。包含在里面以作参考，PME在大多数情况下会表现更好。

coulombtype = PME ;Fast smooth Particle-Mesh Ewald (SPME) electrostatics. Direct space is similar to the Ewald sum, while the reciprocal part is performed with FFTs. Grid dimensions are controlled with fourierspacing and the interpolation order with pme-order. With a grid spacing of 0.1 nm and cubic interpolation the electrostatic forces have an accuracy of 2-3*10^-4. Since the error from the vdw-cutoff is larger than this you might try 0.15 nm. When running in parallel the interpolation parallelizes better than the FFT, so try decreasing grid dimensions while increasing interpolation. 快速平滑粒子-网格Ewald (SPME)静电学。直接空间和Ewald sum相似，然而，倒空间是在FFTs中完成的。

coulombtype = 

coulombtype = 

coulombtype = 

coulombtype = 

coulombtype = 

coulombtype = 

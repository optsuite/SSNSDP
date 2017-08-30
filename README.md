# SSNSDP version 0.1
A MATLAB software for general SDP probelms including 2-RDM problems.

# Problems and solvers
- The package contains codes for general SDP problems including 2-RDM problems:   
   (P) max <C,X> s.t. A(X) = b, X in K,  
    (D) min b^Ty s.t. S = At(y) - C, S in K,  
    where K is a positive semidefinite cone.
- The package can deal with SDP problems under the format of [SDPNAL](http://www.math.nus.edu.sg/~mattohkc/SDPNAL.html). The authors are grateful to Prof. Kim Chuan Toh and Prof. Defeng Sun for sharing their source codes.
- Since we mainly consider the 2-RDM problem, the performance of SSNSDP on general problems needs to be further improved.
- A preprocessed 2-RDM data stored in Matlab files can be found at <http://bicmr.pku.edu.cn/~wenzw/code/RDM_matlab_sparse_new.zip>. The original datasets are provided by Prof. Nakata Maho and Prof. Mituhiro Fukuta. One can find parts of the original data from the Website <http://nakatamaho.riken.jp/rdmsdp/sdp_rdm.html>. The process code is `[blk_new,At_new,C_new,c,hists] = rdm_detect_block(blk,At,C,b)`

# References
- [Yongfeng Li, Zaiwen Wen, Chao Yang, Yaxiang Yuan, A Semi-smooth Newton Method for Solving Semidefinite Programs in Electronic Structure Calculations, arXiv:1708.08048](https://arxiv.org/abs/1708.08048)
- [Xiantao Xiao, Yongfeng Li, Zaiwen Wen, Liwei Zhang, A Regularized Semi-Smooth Newton Method With Projection Steps for Composite Convex Programs, arXiv:1603.07870](https://arxiv.org/abs/1603.07870)
- [Zaiwen Wen, Donald Goldfarb, Wotao Yin, Alternating direction augmented Lagrangian methods for semidefinite programming, Mathematical Programming Computation,  Vol 2, Issue 3–4, pp 203–230, 2010](https://link.springer.com/article/10.1007/s12532-010-0017-1)

# The Authors
We hope that the package is useful for your application.  If you have any bug reports or comments, please feel free to email one of the toolbox authors:

* Yongfeng Li, yongfengli at pku.edu.cn
* Zaiwen Wen, wenzw at pku.edu.cn

# Installation
`>> Installmex_ssm`  
`>> startup(your_data_path)`  
`>> cd example`  
`>> demo`  


# Copyright
 -------------------------------------------------------------------------
  Copyright (C) 2017, Yongfeng Li, Zaiwen Wen

  This program is free software: you can redistribute it and/or modify
  it under the terms of the GNU General Public License as published by
  the Free Software Foundation, either version 3 of the License, or
  (at your option) any later version.

  This program is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without  even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  GNU General Public License for more details.

  You should have received a copy of the GNU General Public License
  along with this program.  If not, see <http://www.gnu.org/licenses/>


<p align="right">
  <a href="hphc-teukolsky-solver.md"><img src="https://img.shields.io/badge/English-English-6e7781?style=flat-square" alt="English"></a>
</p>

<p align="center">
  <a href="../README.zh-CN.md"><img src="https://img.shields.io/badge/%E8%BF%94%E5%9B%9E-%E4%B8%AD%E6%96%87%E4%B8%BB%E9%A1%B5-24292f?style=flat-square" alt="返回中文主页"></a>
</p>

<h1 align="center">HPHC 坐标下的 Teukolsky 方程时域求解器</h1>

<p align="center">
  <b>Horizon-Penetrating Hyperboloidally Compactified Teukolsky Evolution</b>
</p>

---

## 概述

我们开发了基于 **horizon-penetrating, hyperboloidally compactified (HPHC) coordinates** 的 Teukolsky 方程独立时域求解器。

该方法在从黑洞视界到未来零无穷 $\mathcal{I}^{+}$ 的紧致化区域上演化 spin-$s$ Teukolsky 方程，使得可以直接在零无穷处提取 retarded waveform，而无需额外的大半径外推。

## 功能

- HPHC 坐标下的双曲演化
- 在未来零无穷 $\mathcal{I}^{+}$ 直接提取波形
- Kerr 时空演化
- $m$-mode 分解
- $2+1$ 维演化
- NVIDIA GPU 加速
- 局域源项支持

## 应用

该求解器被用于频域 Green's function decomposition 计算的独立时域验证。

在 Kerr Green's function decomposition 工作中，该工具用于比较直接时域演化得到的 $\mathcal{I}^{+}$ 波形与由 direct wave 和 quasinormal-mode contribution 重构得到的波形。

该工具的技术描述见：

> J. Su, N. Khera, A. Chowdhuri, M. Casals, and H. Yang,  
> *Gravitational Waves from Green's Function Decomposition for a Kerr Black Hole: I. Equatorial ISCO Plunge*  
> arXiv:2608.17943

## 获取方式

该时域求解器目前仍在封装和维护中，后续工作仍会继续使用和扩展该工具。

因此短时间内不会公开代码。待代码维护、文档和封装工作达到合适阶段后，将可能通过邮件申请方式提供。

---

<p align="center">
  <a href="../README.zh-CN.md"><img src="https://img.shields.io/badge/%E8%BF%94%E5%9B%9E-%E4%B8%AD%E6%96%87%E4%B8%BB%E9%A1%B5-24292f?style=flat-square" alt="返回中文主页"></a>
</p>

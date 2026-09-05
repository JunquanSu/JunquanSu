<p align="right">
  <a href="frequency-domain-solvers.md"><img src="https://img.shields.io/badge/English-English-6e7781?style=flat-square" alt="English"></a>
</p>

<p align="center">
  <a href="../README.zh-CN.md"><img src="https://img.shields.io/badge/%E8%BF%94%E5%9B%9E-%E4%B8%AD%E6%96%87%E4%B8%BB%E9%A1%B5-24292f?style=flat-square" alt="返回中文主页"></a>
</p>

<h1 align="center">频域求解器</h1>

<p align="center">
  <b>Regge–Wheeler–Zerilli · Teukolsky · Sasaki–Nakamura</b><br>
  支持复频率的黑洞微扰径向与角向求解工具
</p>

---

## 概述

我们开发了 **Regge–Wheeler–Zerilli**、**Teukolsky** 和 **Sasaki–Nakamura** 方程的齐次求解器。这些求解器可在较大的参数空间中可靠计算径向解和渐近振幅，尤其针对较大复频率区域进行了处理。

## 功能

- Regge–Wheeler–Zerilli 齐次径向解
- Teukolsky 齐次径向解
- Sasaki–Nakamura 齐次径向解
- Teukolsky 方程的角向解
- 分离常数
- 渐近振幅
- 复频率计算（解析延拓）

## 数值可靠性

我们特别关注复杂频率平面上的数值稳定性与可靠性，同时保持适合较大规模计算的效率。

在我们的测试中，一些现有公开实现用于复频率时会出现较隐蔽但重要的问题。例如，[Black Hole Perturbation Toolkit](https://bhptoolkit.org/index.html) 中的部分工具在复频率平面的某些区域可能出现标准实频计算中不易察觉的问题。我们也发现 `GeneralizedSasakiNakamura.jl` 在 $\omega$ 平面靠近虚轴的区域会变得不可靠，并且在复频率时可能给出错误的径向解和角向解。

这些问题促使我们开发独立的数值工具，并将复杂频率平面上的稳健性作为重点。

## 获取方式

出于实际原因，这套频域求解器短期内不会公开源代码。如需使用代码或进行数值结果对比，可以通过邮件与我联系。

---

<p align="center">
  <a href="../README.zh-CN.md"><img src="https://img.shields.io/badge/%E8%BF%94%E5%9B%9E-%E4%B8%AD%E6%96%87%E4%B8%BB%E9%A1%B5-24292f?style=flat-square" alt="返回中文主页"></a>
</p>

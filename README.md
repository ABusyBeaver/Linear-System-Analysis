# MATLAB 线性系统分析 (Linear-System-Analysis) 工具

[![MATLAB](https://img.shields.io/badge/MATLAB-R2020a%2B-blue?logo=mathworks)](https://www.mathworks.com/products/matlab.html)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Control System Toolbox](https://img.shields.io/badge/Control_System_Toolbox-required-orange)](https://www.mathworks.com/products/control.html)

**一个基于 MATLAB App Designer 开发的综合性控制系统分析平台**，整合频域分析、时域分析、根轨迹分析和系统校正四大核心模块，为控制工程教学、科研和工程应用提供直观、高效的线性时不变（LTI）系统分析环境。

## ✨ 主要特点

- 支持传递函数模型快速创建与参数配置
- 提供频域（Bode 图、Nyquist 图、稳定裕度）、时域（阶跃/脉冲/斜坡响应）、根轨迹全面分析
- 集成超前补偿器与滞后补偿器自动设计算法
- 图形界面与算法实时交互，支持参数即时调整与可视化反馈
- 完善的错误处理与多级用户提示系统
- 采用面向对象编程，代码结构清晰，易于维护和二次开发

## 📥 安装与运行

### 环境要求
- MATLAB R2020a 及以上版本
- Control System Toolbox（控制系统工具箱）

### 运行步骤
1. 下载`LSA.mlapp` 文件
2. 双击，待工具界面启动后即可开始使用

## 🚀 核心功能

### 系统建模
输入分子和分母系数，点击“创建系统”按钮即可生成传递函数模型。

### 频域分析
- Bode 图：自动绘制幅频与相频特性曲线，并计算增益裕度和相位裕度
- Nyquist 图：绘制奈奎斯特曲线并标注临界点(-1,0)
  
### 时域分析
支持阶跃响应、脉冲响应、斜坡响应，自动计算超调量、上升时间、调节时间、稳态值等性能指标。

### 根轨迹分析
支持开环与闭环根轨迹绘制，可标记指定增益下的闭环极点。

### 系统校正
- 超前补偿器设计（基于目标相位裕度）
- 滞后补偿器设计（基于稳态误差要求）
- 校正后效果实时验证

## 🏗️ 系统架构

LSA 工具基于 MATLAB App Designer 开发，主类继承自 matlab.apps.AppBase，核心数据流围绕 sys_tf展开

## 📸 界面截图

<table align="center">
  <tr>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/563d24e9-340c-43ed-b818-6a2b130fdd28" width="360"><br>
      <sub><b>频域分析</b></sub>
    </td>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/ea13648b-2296-4673-9b2b-7ad497fa8747" width="360"><br>
      <sub><b>时域分析</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/9ca5a19e-14f4-42d0-9212-86ee6c7c4a97" width="360"><br>
      <sub><b>根轨迹分析</b></sub>
    </td>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/2d53c897-20c7-4d99-92db-3e473e20ac6b" width="360"><br>
      <sub><b>补偿器设计</b></sub>
    </td>
  </tr>
</table>
















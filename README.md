# Biomedical-Optics-Papers
 Scientific Papers Related to Biomedical Optics Imaging

## Research Interests:

1. Optical Coherence Tomography
2. Optical Mapping of Cardiac Electrophysiology
3. Fluorescence Microscopy
4. Bragg Grating Fiber Shape Sensing
5. Imaging in Highly Scattering Medium

## Papers

### Optical Coherence Tomography

### Optial Mapping of Cardiac Electrophysiology

--- 
- **Spectral characteristics of voltage-senstive indocyanine green fluorescence in the heart**
- 2017 / Sci. Rep. / Regina Mačianskienė
- DOI:10.1038/s41598-017-08168-7
- 揭示ICG电压敏感染料在心脏中发出荧光的工作原理. 
- 最简单的理解是, 使用荧光染料对生物样本进行染色后, 荧光染料所激发的强度会随着某种生物过程变化而变化. 当使用一个固定强度的激发光(excitation)去照射荧光染色后的样本, 其会产生一个波长更长的出射光(emission). 使用光传感器(如相机等), 就可以通过光的变化捕捉该生物过程的变化. 
- 具体到这篇文章中, ICG是一种FDA认证的电压敏感染料, 可以反映样本中生物电的变化. 当心脏的电生理过程发生变化时, 就可以通过出射光的强度反映心脏的电位变化. 
- 本文中使用了四个波段的LED光来获得激发, 用以研究ICG染料对于不同激发波段的荧光响应. 
--- 
- **Understanding Clinical Cardiac Electrophysiology**
- Wiley Backwell / Peter Spector
- https://onlinelibrary.wiley.com/doi/book/10.1002/9781118905500
- 讲述心脏电位过程的教材.
- 
--- 
- **Optical mapping of contracting hearts**
- The Journal of Physiology / Vineesh Kappadan 
- DOI: 10.1113/JP283683
- 使用运动追踪算法和比值法测量来弥补心脏光学标定中的运动伪影
- 心脏光学标定的基本实验配置是对应荧光染料的LED波长照射心脏, 心脏中的荧光染料根据生理电位的变化产生更长波长的荧光信号, 其强度随电位变化而变化. 再通过一片激发滤光片滤掉干扰荧光信号的杂散光, 最后通过一个光电探测器获取图像. 
- 在心脏电位的光学标定中, 有三个导致运动伪影的因素: 心脏和探测器之间的相对运动; 不均匀的荧光染料分布; 不均匀的光照. 

--- 
- **Lenses and effective spatial resolution in macroscopic optical mapping**
- PHYSICS IN MEDICINE AND BIOLOGY / Harold Bien
- Phys. Med. Biol. 52 (2007) 1–21
- 描述了荧光光学标定中与其他成像方式的不同: 动态范围, 低荧光信号等. 
- 传统的光学系统的空间分辨极限是通过衍射极限确定的, 或者是通过探测器像素经过光学系统成像后的尺寸决定的. 但是这种情况仅仅确定了空间分辨率的上限, 未考虑物体与背景之间的光强差异, 以及样本, 探测器的特性. 这几种传统成像未考虑的影响因素, 作者通过对比度概述, 然后再用CTF(contrast transfer function)和轴向分辨率与横向分辨率定量描述. 
- 荧光光学标定与传统光学成像应用不同, 其主要会受到空间限制的影响. 对比度受限的成像(如生物荧光光学标定)会对成像效果有如下影响: 1. 透镜或镜头等光学元件会降低对比度, 进而导致分辨率下降. 这是工程光学中已经清楚描述的, 具体参考光学系统的像质评价. 2. 最小可分辨的对比度对应为数字图像上最小划分的灰度值, 这点通常在传统成像应用中忽略. 3. 成像系统的实际分辨能力是被测物体的对比函数. 除了这三种因素外, 还需要考虑三维物体的荧光是如何投射到平面成像传感器上的, 此时还需考虑到轴向分辨率对对比度的限制. 
- CTF和MTF的不同之处在于前者描述黑白二元图样, 后者则是对空间频率的正弦调制响应. 这两个特性都可以从理论上计算为已知光学元件特性的线扩展函数的傅里叶变换的幅度, 测试的方法就是对不同空间频率的样本进行成像(如USAF空军分辨率板等), 两者的关键简述为文中(2)式: 
- $MTF = 0.785*CTF(v)$
- 单色衍射极限调制传递函数与透镜数值孔径的关系可以描述为: 
- $MDMTF(v)\, =\frac {2} {\pi }(\phi -cos\phi sin\phi )$
- $\phi ={cos}^{-1}(\frac {\lambda v} {2NA})$
- 适用于荧光成像系统的CTF和MTF应该可以通过经验测量确定. NA可以通过上两式确定. 
- 背景噪声则是通过MTF和信号峰-峰值确定. 求解的值即为能分辨的最小灰度值. 系统可解析的最高空间频率 ${v}_{max}$等同于信噪比的倒数, 或者是信号峰-峰值的倒数. 
- 景深是指光学系统能够对三维组织收集清晰光的范围. 景深确定的公式为: 
- $DOF=\frac {\lambda *n} {{NA}^{2}}+\frac {n} {M*NA}e$, 其中e为采样像素大小, M为放大倍率. 据此公式计算, 理论景深为0.2861mm. 显微镜物镜给出的实际景深为0.11mm. 所以当考虑到探测器和镜头数值孔径后, 计算出来的景深似乎会比厂商给出的景深稍大. 
- 镜头选型中, 需要考虑的参数包括焦距, F数, 放大倍率. 具体公式参考文献中的(16)
> 有用的结论: 数值孔径不能仅作为镜头分辨率的判据. 
> 
> 对比度依赖于有效光信息和曝光时间. 这个是我们实验验证得出来的结论, 这篇论文提供了理论支撑. 
> 
> 光学标定中的横向分辨率依赖于染料质量以及其信噪比. 
>
> 焦距较短的镜头会限制成像的轴向分辨率, 轴向空间分辨率受到从焦平面到低于本底噪声点的距离处的强度损失的限制. 但是这个轴向分辨率的限制对于宏观成像的影响应该不大. 

--- 
- **Correction of motion artifact in transmembrane voltage-sensitive fluorescent dye emission in hearts**
- Heart and circulatory physiology
- 10.1152/ajpheart.00574.2003.
- 给出了比值法测量心脏膜电位的公式分析. 
- 光电探测器获得的荧光信号为$S_i(t)=I(t)(E_i+D_i)$, 其中I为荧光强度, E为荧光变化, D为背景. E和D都是归一化后的值, 则I为归一化的强度系数. 
- 荧光变化$E_i=F_i(t)M_i(t)C_i(t)$, 其中F为膜电位信号, M为运动影响, C为荧光强度的随时间漂白. 
- 膜电位信号$F_i(t)=A_i[1+a_iV_m(t)]$, 其中A和a都是和照射波长有光的参量, V是膜电位. 
- 运动影响$M_i(t)=1+b_iM(t)$, 其中b为与波长相关的参量, M为运动. 
- 这样, 光电探测器采集到的信号就可以表示为$S_i(t)=I(t)\{A_i[1+a_iV_m(t)][1+b_iM(t)]C_i(t)+D_i\}$
- 这个公式中的噪声, 应该可以使用拍摄无荧光信号的参考图像, 然后使用有荧光信号的图像减去即可去掉. 这个方法在其他领域也有用到, 那么拍摄配置就是一个拍摄周期拍三张图片: 较高波长照明, 较低波长照明, 以及一个无波长照明的. 
- 去掉背景后, 使用比值法. 得到比值后的信号${S}^{\ast }_{1/2}(t)={S}^{\ast }_{1}(t)/{S}^{\ast }_{2}(t)=A_1I(t)C_1(t)[1+a_1V_m(t)][1+b_1M(t)]/A_2I(t)C_2(t)[1+a_2V_m(t)][1+b_2M(t)]$, 其中${S}^{\ast }$表示去噪后的信号. 
- 文中使用泰勒级数展开化简, 为${S}^{\ast }_{1/2}(t)=H_1(t)/H_2(t)[1+(a_1-a_2)V_m(t)][1+(b_1-b_2)M(t)]$, 其中$H_t(t)=A_iI_i(t)C_i(t)$. 
- 若机械运动造成的影响可以忽略, 那么${S}^{\ast }_{1/2}(t)=k[1+(a_1-a_2)V_m(t)]$. 
- 这样, 这个公式就可以解释我们实验中的部分现象了. 具体的就不在此详写了. 

--- 
- ****
- 

--- 
- ****
- 
- 


### Fluorescence Microscopy

### Bragg Grating Fiber Shape Sensing

--- 
- ****
- 
- 
--- 
- ****
- 
- 
--- 
- ****
- 

--- 
- ****
- 

--- 
- ****
- 

--- 
- ****
- 

--- 
- ****
- 
- 



### Imaging in Highly Scattering Medium

---
- **Optical imaging through dynamic turbid media using the Fourier-domain shower-curtain effect**
- 2016 / Optica / Eitan Edrei et al. 
- https://doi.org/10.1364/OPTICA.3.000071
---
- **Reconstruction of an object from the modulus of its Fourier transform**
- 1978 / OL / J.R.Fienup
- https://doi.org/10.1364/OL.3.000027
--- 
- **Deep optical imaging within complex scattering media**
- 2020 / nature physics review / Seokchan Yoon et al.
- https://www.nature.com/articles/s42254-019-0143-2


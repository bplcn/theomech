@def title = "力系的简化"
@def hascode = true
@def date = Date(2022, 8, 26)
@def rss = "力系的简化"

@def tags = ["syntax", "code"]

# 力系的简化
## 2-1 力系的分类
### 1. 汇交力系
定义：力系中各力作用线汇交于一点，则该力系称为**汇交力系**。汇交力系有时也称为共点力系。

如果一个汇交力系的各力的作用线都位于同一平面内，则该汇交力系称为**平面汇交力系**，否则称为**空间汇交力系**。

汇交力系案例

### 2. 力偶系
定义：作用在物体上的一群力偶称为力偶系（couple system）。 
      
若力偶系中的各力偶都位于同一平面内，则为平面力偶系，否则为空间力偶系。 

### 3. 任意力系
定义：若力系中各力的作用线既不汇交于一点，又不全部相互平行，则该力系称为任意力系。 

如各力作用线还位于同一平面内，则称为平面任意力系，简称平面力系；否则称为空间任意力系，简称空间力系。 


## 2-2 力的平移定理（重点难点）
附加力偶：$M = F\cdot a = M_B(\overrightarrow{F}_A)$

> 作用在刚体上的力，可以等效地平移到刚体上任一指定点，但必须在该力与指定点所确定的平面内附加一个力偶，附加力偶的力偶矩等于原力对指定点的力矩。 

$\overrightarrow{\boldsymbol{M}}$,$\overrightarrow{\boldsymbol{F}}_B$组成的力系常称为共面的一个力和一个力偶。

## 2-3 力系的简化
### 一、汇交力系的简化 
#### 1. 汇交力系合成的几何法 
$$
\overrightarrow{\boldsymbol{F}}_{R1} = \overrightarrow{\boldsymbol{F}}_{1} + \overrightarrow{\boldsymbol{F}}_{2}
$$

$$
\overrightarrow{\boldsymbol{F}}_{R2} = \overrightarrow{\boldsymbol{F}}_{R1} + \overrightarrow{\boldsymbol{F}}_{3} = \sum_{i=1}^{3}\overrightarrow{F}_i
$$

#### 2. 汇交力系合成的解析计算

$$
\overrightarrow{\boldsymbol{F}}_i = F_{ix}\overrightarrow{\boldsymbol{i}} + 
    F_{iy}\overrightarrow{\boldsymbol{j}} + F_{iz}\overrightarrow{\boldsymbol{k}}
$$

#### 2. 汇交力系合成的解析法 
$$
\overrightarrow{\boldsymbol{F}}_R = \left(\sum F_{ix}\right)\overrightarrow{\boldsymbol{i}} 
    + \left(\sum F_{iy}\right)\overrightarrow{\boldsymbol{j}}
    + \left(\sum F_{iz}\right)\overrightarrow{\boldsymbol{k}}
$$

矢量投影定理（重点难点）：
$$
    \left.\begin{split}
        F_{Rx} = \sum F_{ix}
        F_{Ry} = \sum F_{iy}
        F_{Rz} = \sum F_{iz}
    \end{split}\right\}
$$

$$
    \left.\begin{split}
        F_{R} = \sqrt{F_{Rx}^2+F_{Ry}^2+ F_{Rz}^2}  \\
        \cos \left(\overrightarrow{\boldsymbol{F}}_R,x\right)=\frac{F_{Rx}}{F_R}   \\
        \cos \left(\overrightarrow{\boldsymbol{F}}_R,y\right)=\frac{F_{Ry}}{F_R}   \\
        \cos \left(\overrightarrow{\boldsymbol{F}}_R,z\right)=\frac{F_{Rz}}{F_R} 
    \end{split}\right\}
$$
> 如果所研究的力系是**平面汇交力系**，取力系所在平面为平面，则该力系的合力的大小和方向只需将$F_{Rz}=0$ 代入式中便可求得。 

### 二、力偶系的简化 


### 三、任意力系的简化 
#### 1、平面任意力系向作用面内一点简化·主矢和主矩
原力系的主矢量
$$
\overrightarrow{\boldsymbol{F}_R} = \sum \overrightarrow{\boldsymbol{F}_i^\prime} + \overrightarrow{\boldsymbol{F}_R}
$$
原力系对O点的主矩
$$
M_O = \sum M_0(\overrightarrow{\boldsymbol{F}_i^\prime})
$$
主矢与简化中心无关，而主矩一般与简化中心有关。
主矢量和主矩的解析计算：
$$
\begin{split}
F_{Rx} = \sum F^\prime_{ix} = \sum F_{ix} 
F_{Ry} = \sum F^\prime_{iy} = \sum F_{iy} 
\end{split}
$$
主矢大小：$F_R = \sqrt{ F_{Rx}^2 + F_{Ry}^2 }$
主矢方向：$\cos \left(\overrightarrow{\boldsymbol{F}}_R,\overrightarrow{\boldsymbol{i}}\right)=\sum F_{ix}/F_R, \cos \left(\overrightarrow{\boldsymbol{F}}_R,\overrightarrow{\boldsymbol{i}}\right)=\sum F_{iy}/F_R$，作用在简化中心上。

简化结果讨论

| 主矢 | 主矩 | 最终结果 | 说明 |
| :---: | :---: | :---: | :---: |
| $\overrightarrow{\boldsymbol{F}_R} \neq 0$ | $M_O = 0$ | 合力 | 合力作用线过简化中心 |
| $\overrightarrow{\boldsymbol{F}_R} \neq 0$ | $M_O \neq 0$ | 合力 | 合力作用线距简化中心距离？|
| $\overrightarrow{\boldsymbol{F}_R} = 0$ | $M_O \neq 0$ | 合力 | 与简化中心的位置无关 |
| $\overrightarrow{\boldsymbol{F}_R} = 0$ | $M_O = 0$ | 平衡 | 与简化中心的位置无关 |


------
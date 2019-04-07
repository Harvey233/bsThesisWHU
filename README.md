武汉大学本科毕业论文模板
==============
本项目包含如下内容：
##论文LaTex模板
主要包含三部分
- bsThesisWHU.tex 为主文件，直接打开写作即可。
- data文件夹
包括导言区设置文件 preamble.tex 和 正文前的声明、摘要、目录页等设置文件frontmatter.tex。可将主文件中的章节文件单独置于此文件夹内，以便集中精力写作。
- figures文件夹放置图形文件

##本科论文Word模板
word模板，按照模版内说明使用即可

##官方本科论文规范
本科生院对于毕业论文的要求：http://ugs.whu.edu.cn/info/1049/1935.htm

##本科论文要求.pdf
重新排版后的官方要求，方便查阅
---
Updated on 2015-05-16

以下内容由Zhangjie Lyu更新：

不冲突地加入头文件（所有注释的代码都可能发生冲突，显著更改格式）
\documentclass[a4paper,fancyhdr,fntef,UTF8,hyperref,openany,oneside,notitlepage]{book}%%,adobefonts
\input{data/preamble}%导言区设置命令单独放在data文件夹下的preamble.tex文件中
% \usepackage{CJK}
% \usepackage{ctex}
\usepackage{amsmath,amssymb,amstext} %多种公式环境和数学命令
\usepackage{float}
% \usepackage[utf8]{inputenc}
\usepackage{array}           %数组和表格制作
\usepackage{fancyhdr}        %页眉页脚设置
\usepackage{graphicx}        %插图
\usepackage{tabularx}
\usepackage{booktabs}
%自动设置表格列宽
\usepackage{multirow}        %跨行表格
\usepackage{multicol}        %跨列表格
% \usepackage{titlesec}        %标题设置
% \usepackage{titletoc}        %目录格式设置
\usepackage{caption}
\usepackage{subcaption}
\usepackage{enumerate}
\usepackage{bbm}

% \usepackage[top=0.8cm,bottom=1.5cm,left=1.5cm,right=1.5cm]{geometry} % 页边距
% \newcommand{\hei}{\CJKfamily{hei}}  %定义的新命令
% \newcommand{\li}{\CJKfamily{li}}
% \renewcommand{\figurename}{{图}}
% \linespread{1.3}   %1.5倍行距
\usepackage{listings}
% \usepackage{xcolor}
%   \lstset{numbers=left, %设置行号位置
%         numberstyle=\tiny, %设置行号大小
%         keywordstyle=\color{blue!70}, %设置关键字颜色
%         commentstyle=\color[cmyk]{1,0,1,0}, %设置注释颜色
%         frame=shadowbox, %设置边框格式
%         rulesepcolor=\color{red!20!green!20!blue!20},
%         escapeinside=``, %逃逸字符(1左面的键)，用于显示中文
%         breaklines, %自动折行
%         extendedchars=false, %解决代码跨页时，章节标题，页眉等汉字不显示的问题
%         xleftmargin=2em,xrightmargin=2em, aboveskip=1em, % 设置边距
%         %tabsize=4, %设置tab空格数
%         %showspaces=false %不显示空格
%       }

\usepackage{natbib}
\setcitestyle{numbers}

\begin{document}

不冲突的加入bib文件型附录而不是使用\bibitem{}命令
\clearpage\phantomsection
\addcontentsline{toc}{chapter}{参考文献}
\renewcommand{\bibname}{参考文献}
\bibliographystyle{plain}
\bibliography{reference}

\addcontentsline{toc}{chapter}{致谢}
\chapter*{致谢}

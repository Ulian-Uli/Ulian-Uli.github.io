<h1>🧬 基本概念</h1>
<h2>1️⃣ 高通量测序</h2>
<p>一种能同时对数百万条 DNA 或 RNA 分子进行快速测序的技术，可一次性获得海量基因序列信息<br>
就像一台<strong>高速扫描仪</strong>，把样本里所有的基因蓝图一次性读取出来，生成庞大的“原始数据报告”</p>
<h2>2️⃣ 生物信息学（生信分析）</h2>
<p>利用<strong>计算机+统计学</strong>来管理、分析和解读生物学数据（尤其是高通量测序结果）<br>
好比一位数据分析师，把“原始报告”整理计算，最终告诉我们<strong>哪些基因最关键、意味着什么</strong></p>
<h2>3️⃣ 差异表达基因（DEGs）</h2>
<p>在不同条件（如<strong>癌组织 vs 正常组织</strong>）下，<strong>表达量存在显著统计学差异</strong>的基因<br>
常用筛选标准：<code inline="">adj.P.value &lt; 0.05</code> 且 <code inline="">|log2FC| &gt; 2</code></p>
<ul>
<li>
<p>adj.P.value：校正后的 P 值 &lt; 0.05</p>
</li>
<li>
<p>|log2FC| &gt; 2：表达量变化超过 <strong>4 倍</strong></p>
</li>
</ul>
<h2>4️⃣ GO 分析</h2>
<p><strong>Gene Ontology</strong>：国际标准的基因功能分类体系，从三个维度描述基因的功能：</p>
<ul>
<li>
<p><strong>BP</strong>（Biological Process）：生物学过程，如“细胞分裂”</p>
</li>
<li>
<p><strong>CC</strong>（Cellular Component）：细胞内的具体位置</p>
</li>
<li>
<p><strong>MF</strong>（Molecular Function）：分子水平的具体活性</p>
</li>
</ul>
<blockquote>
<p>本研究中发现：这些基因显著富集于<strong>有丝分裂细胞周期</strong>、脂质颗粒和蛋白质二聚化等过程——这与癌细胞的高增殖、高代谢特征高度一致</p>
</blockquote>
<h2>5️⃣ KEGG 通路分析</h2>
<p><strong>Kyoto Encyclopedia of Genes and Genomes</strong><br>
用于解析基因产物之间的<strong>相互作用网络</strong>并映射到具体信号通路<br>
本研究中关键结果示例：</p>
<ul>
<li>
<p><strong>PPAR 通路</strong>：调节细胞脂质/葡萄糖代谢，提示乳腺癌存在<strong>代谢重编程</strong></p>
</li>
<li>
<p><strong>AMPK 通路</strong>：细胞能量感受器；癌细胞可能破坏了这种“能量刹车”</p>
</li>
<li>
<p><strong>ECM 受体相互作用</strong>：与<strong>肿瘤侵袭转移</strong>密切相关</p>
</li>
</ul>
<h2>6️⃣ 蛋白互作网络（PPI）&amp; Degree 值</h2>
<ul>
<li>
<p>PPI：用网络图展示蛋白质的相互作用，一个<strong>节点</strong>代表一个蛋白，一条<strong>连线</strong>代表已知或预测的相互作用</p>
</li>
<li>
<p>Degree 值：节点直接连接的数量。值越高，表示该蛋白在网络中越<strong>核心</strong>，潜在治疗靶点价值越大</p>
</li>
</ul>
<blockquote>
<p>研究发现核心基因为 <strong>FOXM1、UBE2C、CDKN3</strong></p>
<ul>
<li>
<p><strong>FOXM1</strong>：调控细胞周期的著名原癌基因</p>
</li>
<li>
<p><strong>UBE2C</strong>：泛素结合酶，推动细胞周期进程</p>
</li>
<li>
<p><strong>CDKN3</strong>：细胞周期调节因子，某些癌症中可能发挥促癌作用</p>
</li>
</ul>
</blockquote>
<h2>7️⃣ 磷酸化</h2>
<p>可类比为<strong>给蛋白质插钥匙启动</strong><br>
AKT 等激酶在磷酸化后结构改变，被“点火”而激活，从而驱动下游信号传导</p>
<hr>
<h1>📑 论文总结</h1>
<h2>1️⃣ 基本文献信息</h2>

项目 | 内容
-- | --
标题 | 基于生物信息学筛选乳腺癌差异表达基因 UBE2C 及其功能验证
作者 | 芦梓楠
导师 | 孙刚 教授/主任医师
学校 | 新疆医科大学
学位 | 医学硕士论文
专业方向 | 肿瘤学（乳腺癌病因及分子机制）
年份 | 2021年3月
期刊 | 硕士学位论文（未发表期刊）


<hr>
<h2>2️⃣ 研究背景</h2>
<ul>
<li>
<p>乳腺癌是全球女性<strong>最常见恶性肿瘤</strong>之一，发病率持续上升</p>
</li>
<li>
<p><strong>UBE2C</strong> 在多种肿瘤中高表达，与细胞周期调控和肿瘤增殖密切相关，但其在乳腺癌中的具体机制尚不明确</p>
</li>
<li>
<p>高通量测序与生物信息学有助于挖掘差异表达基因，为<strong>诊断标志物</strong>和<strong>治疗靶点</strong>提供新思路</p>
</li>
</ul>
<h2>3️⃣ 研究目的</h2>
<ol>
<li>
<p><strong>生信分析</strong>：基于 GEO + TCGA 数据库筛选乳腺癌差异表达基因，挖掘核心基因</p>
</li>
<li>
<p><strong>功能验证</strong>：通过细胞实验验证 UBE2C 的生物学作用及分子机制</p>
</li>
</ol>
<h2>4️⃣ 研究方法</h2>
<h3>Part I：生物信息学分析</h3>
<ul>
<li>
<p>数据来源：GEO（GSE21422、GSE45827、GSE70947）、TCGA</p>
</li>
<li>
<p>差异基因筛选：adj.P.value &lt; 0.05 且 |log2FC| &gt; 2</p>
</li>
<li>
<p>功能富集：GO &amp; KEGG（发现 PPAR、AMPK、ECM 通路）</p>
</li>
<li>
<p>PPI 网络：筛选核心基因 FOXM1、UBE2C、CDKN3</p>
</li>
<li>
<p>生存分析：UBE2C 高表达患者的无复发生存率显著降低（HR=1.83，P&lt;0.001）</p>
</li>
</ul>
<h3>Part II：UBE2C 功能验证</h3>
<ul>
<li>
<p>细胞株：MDA-MB-231（高侵袭三阴性）、MCF-7（雌激素受体阳性）</p>
</li>
<li>
<p>实验：siRNA 沉默 UBE2C → RT-qPCR → CCK-8 → Transwell → Western blot</p>
</li>
<li>
<p>指标：细胞增殖、侵袭能力、AKT/mTOR 信号通路相关蛋白磷酸化水平</p>
</li>
</ul>
<h2>5️⃣ 主要结果</h2>
<ul>
<li>
<p><strong>生信分析</strong>：共筛得 151 个乳腺癌差异表达基因，UBE2C 与患者预后显著相关</p>
</li>
<li>
<p><strong>细胞实验</strong>：敲低 UBE2C 后，细胞增殖与侵袭显著下降；Western blot 显示 p-PTEN 升高，p-AKT、p-mTOR、HIF-1α 下调</p>
</li>
</ul>
<h2>6️⃣ 结论</h2>
<ul>
<li>
<p><strong>UBE2C 在乳腺癌中高表达</strong>，其高表达提示患者预后较差</p>
</li>
<li>
<p>UBE2C 通过激活 <strong>AKT/mTOR 信号通路</strong>促进乳腺癌细胞增殖和侵袭，是潜在的<strong>治疗靶点</strong></p>
</li>
</ul>
<blockquote>
<p>🔑 <strong>一句话总结</strong><br>
GEO+TCGA 生信分析 + 体外实验共同证明：<strong>UBE2C 是乳腺癌核心致癌基因，通过 AKT/mTOR 通路促进肿瘤进展</strong></p>
</blockquote>
<hr>
<h1>🧪 实验设计分析</h1>
<h2>实验一：细胞培养与转染</h2>
<ul>
<li>
<p><strong>目的</strong>：用 siRNA 沉默 UBE2C，制造“缺失”模型</p>
</li>
<li>
<p><strong>方法</strong>：Lipofectamine2000 转染 siRNA；设置空白对照、阴性对照及两条 si-UBE2C 组</p>
</li>
<li>
<p><strong>意义</strong>：这是操纵变量的<strong>关键步骤</strong>，为后续验证奠定基础</p>
</li>
</ul>
<h2>实验二：RT-qPCR</h2>
<ul>
<li>
<p><strong>目的</strong>：验证转染是否有效（mRNA 水平）</p>
</li>
<li>
<p><strong>结果</strong>：UBE2C mRNA 明显下降 → 转染成功</p>
</li>
</ul>
<h2>实验三：CCK-8</h2>
<ul>
<li>
<p><strong>目的</strong>：检测细胞增殖能力</p>
</li>
<li>
<p><strong>原理</strong>：活细胞代谢活跃 → 颜色加深 → 450nm 吸光度升高</p>
</li>
<li>
<p><strong>结果</strong>：UBE2C 下调后，增殖曲线显著下降</p>
</li>
</ul>
<h2>实验四：Transwell 侵袭实验</h2>
<ul>
<li>
<p><strong>目的</strong>：评估细胞穿膜能力，模拟肿瘤转移</p>
</li>
<li>
<p><strong>结果</strong>：沉默 UBE2C 后，穿膜细胞数显著减少</p>
</li>
</ul>
<h2>实验五：Western Blot</h2>
<ul>
<li>
<p><strong>目的</strong>：检测 AKT/mTOR 通路关键蛋白的<strong>磷酸化状态</strong></p>
</li>
<li>
<p><strong>结果</strong>：</p>
<ul>
<li>
<p><strong>p-AKT / p-mTOR ↓</strong>：通路活性降低</p>
</li>
<li>
<p><strong>p-PTEN ↑</strong>：抑癌“刹车”增强</p>
</li>
<li>
<p><strong>HIF-1α ↓</strong>：下游效应减弱</p>
</li>
</ul>
</li>
</ul>
<blockquote>
<p><strong>逻辑链</strong>：<br>
操作变量（基因敲低） → 验证操作（RT-qPCR） → 观察表型（增殖/侵袭） → 机制探索（信号通路）</p>
</blockquote>
<hr>
<p>✨ <strong>总结可视化</strong></p>
<pre><code>UBE2C 敲低
   ↓
AKT/mTOR 信号减弱
   ↓
细胞增殖 &amp; 侵袭下降
</code></pre>
<hr>

# 📎其他链接

**格式引文**  
[1] 芦梓楠. 基于生物信息学筛选乳腺癌差异表达基因 UBE2C 及其功能验证 [D]. 新疆医科大学, 2021. DOI: [10.27433/d.cnki.gxyku.2021.000011](https://doi.org/10.27433/d.cnki.gxyku.2021.000011)

**原文链接**  
[知网论文页面](https://kns.cnki.net/kcms2/article/abstract?v=Axm2Bq0K5ft55g6-XIC4-QrCkUaIMcpxk-vSXQqYU8CxJke62XdeX2Yb7j95nI74aZUE5t_EMxLxpYSf3bC27b_kSO0Ku_7o0vAaMugo2jbSi8YcxGcW5v3H2seGj9MhPKcc10gnX7K_yC9-6E5z4Djpj_Z7YvHaoSQLtqdh-JA=&uniplatform=NZKPT)

**详细版笔记**  
[Notion 笔记](https://www.notion.so/250920-UBE2C-27489ba0c4a680dfbc70d1ab07a821af?source=copy_link)

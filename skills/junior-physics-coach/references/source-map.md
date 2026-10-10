# 来源、教材版本与复用边界

这份索引帮助核对物理原理和课程范围，不是学生正在使用的教材。讲解某一题时先看学生提供的原题、图和课本，再打开本题所需的具体来源页。只看过入口页时不能声称核过教材正文、图号或页码。

## 来源优先级

1. **本题事实：**学生上传的题干、题图、实验记录、老师补充条件。图片看不清时暂停依赖该处的判断。
2. **教材口径：**学生实际使用的出版社、修订版、年级、册次及对应具体页。没拿到具体页时只说“教材页待核对”。
3. **课程范围：**[教育部《义务教育课程方案和课程标准（2022年版）》通知](https://www.moe.gov.cn/srcsite/A26/s8001/202204/t20220420_619921.html)所列物理标准；课程标准不能替代教材原文或地方考试评分细则。
4. **普遍物理关系：**OpenStax 的[高中 Physics 教材](https://openstax.org/books/physics/pages/1-introduction)及下表具体章节。该书的范围和数学深度超过中国初中，抽取机制时先删除超纲公式，再与本题教材表述核对。其[内容仓库](https://github.com/openstax/osbooks-physics)标注 CC BY 4.0，改写或复用材料需按原许可证署名；本 skill 的机制卡是重新组织的短摘要，不复制整页。
5. **可视化与模型：**[PhET 模拟](https://phet.colorado.edu/en/simulations)和 [kidslab 初中物理课件](https://github.com/talkincode/kidslab/blob/main/docs/courseware-plan/junior-physics.md)用于观察怎样呈现变量变化；模拟结果是特定模型的输出，不是学生的实验数据。

## 当前教材框架的核对入口

- [人教版义务教育物理八至九年级新教材介绍](https://www.pep.com.cn/xw/zt/hd/12/xjcjs/cz/202409/t20240925_1995627.html)：介绍八上声、光、热，八下力学，九年级能量与电磁等总体安排；这不是某节课本正文。
- [国家中小学智慧教育平台教材入口](https://basic.smartedu.cn/tchMaterial)：先按学段、出版社、年级、册次确认版本，再核对具体页。若页面要求登录或无法读正文，请学生上传手边那一页。
- [textbook-library 目录索引](https://github.com/pengboyjak/textbook-library)：只可辅助定位教材版本和目录；仓库说明其不含教材正文。不能从目录推断题图、课后题或答案。

## 物理原理的具体核对页

| 主题 | 原始页面 | 本 skill 使用位置 |
|---|---|
| 速度、路程、图像 | [OpenStax 2.2](https://openstax.org/books/physics/pages/2-2-speed-and-velocity)、[2.3](https://openstax.org/books/physics/pages/2-3-position-vs-time-graphs) | 运动卡、平均速度题、坐标图 |
| 声的传播与音调 | [OpenStax 13.1](https://openstax.org/books/physics/pages/13-1-types-of-waves)、[14.1](https://openstax.org/books/physics/pages/14-1-speed-of-sound-frequency-and-wavelength) | 声现象卡 |
| 热传递与物态变化 | [OpenStax 11.2](https://openstax.org/books/physics/pages/11-2-heat-specific-heat-and-heat-transfer)、[11.3](https://openstax.org/books/physics/pages/11-3-phase-change-and-latent-heat) | 热现象卡 |
| 平面镜、折射与透镜 | [OpenStax 16.1](https://openstax.org/books/physics/pages/16-1-reflection)、[16.2](https://openstax.org/books/physics/pages/16-2-refraction)、[16.3](https://openstax.org/books/physics/pages/16-3-lenses) | 光学卡、光路作图 |
| 密度和静止液体压强 | [OpenStax 大学物理 14.1](https://openstax.org/books/university-physics-volume-1/pages/14-1-fluids-density-and-pressure) | 密度、液体压强卡；不用其超纲推导 |
| 惯性与摩擦 | [OpenStax 4.2](https://openstax.org/books/physics/pages/4-2-newtons-first-law-of-motion-inertia) | 力学卡、受力分析 |
| 浮力 | [OpenStax College Physics 11.7](https://openstax.org/books/college-physics/pages/11-7-archimedes-principle) | 浮力卡 |
| 机械、功与能 | [OpenStax 9.1](https://openstax.org/books/physics/pages/9-1-work-power-and-the-work-energy-theorem)、[9.2](https://openstax.org/books/physics/pages/9-2-mechanical-energy-and-conservation-of-energy)、[9.3](https://openstax.org/books/physics/pages/9-3-simple-machines) | 杠杆、功率、机械效率卡 |
| 欧姆定律、串并联、电功率 | [OpenStax 19.1](https://openstax.org/books/physics/pages/19-1-ohms-law)、[19.2](https://openstax.org/books/physics/pages/19-2-series-circuits)、[19.3](https://openstax.org/books/physics/pages/19-3-parallel-circuits)、[19.4](https://openstax.org/books/physics/pages/19-4-electric-power) | 电学卡、电路题 |

## 开源仓库怎样使用

- [hermes-edu-skills 的人教版初中物理同步 skill](https://github.com/hezkvectory/hermes-edu-skills/blob/main/skills/textbook-sync/junior-physics-rj-textbook-sync/SKILL.md)使用 MIT 许可，可借其“现象—模型—证据—应用”流程；该仓库主要给学习任务结构，不能当逐节课本或机制数据库。其七年级物理示例不能当作人教版实际进度。
- [kidslab](https://github.com/talkincode/kidslab)声明代码 MIT、课件内容 CC BY 4.0；区分其“已上线”与“未实现”的实验。借鉴变量操作和读数反馈，不直接搬运课件到回答中。
- [PhET 源码说明](https://phet.colorado.edu/en/about/source-code)指出多数具体模拟源码为 GPL；[当前模拟文件许可说明](https://phet.colorado.edu/en/licensing)说明常规 HTML 模拟文件为 CC BY-NC 4.0。引用交互演示链接与复制、嵌入、改造文件是不同动作；实施后者前核对具体许可。

## 写 reference 卡片时的来源记录

每张新卡片记下：`现象名称｜学生教材版本与页（已核时）｜普遍原理的具体 URL｜模拟或原始图的具体 URL（使用时）｜核对日期｜是否为原文、改写或自制示意图`。正文只保留教学所需的短机制，不粘贴整段教材。两个来源冲突时先查模型条件和版本；无法解决就标出未确认之处，不把某个来源强说成唯一答案。

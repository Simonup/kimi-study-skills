# 设计借鉴与边界记录

本文件记录草案借鉴了哪些外部 skill，以及哪些做法没有采用。借鉴的是对话结构与动作，不逐字复制原文；被引用的第三方 skill 并未对本草案进行审核或背书。

| 外部 skill | 借鉴的具体做法 | 没有采用的部分 |
|---|---|---|
| [wuraaang / active-listening](https://github.com/wuraaang/claude-code-skills/blob/main/active-listening/SKILL.md) | 复述事实、试探性地反映感受、用澄清问题核对、允许留白；在给办法前先取得许可。 | 不采用对谈话者的打分、固定“沉默秒数”或从文字推断身体语言；它也没有青少年或LGBT专门流程。 |
| [harrylabsj / relationship-lab](https://clawhub.ai/harrylabsj/skills/relationship-lab) | 在使用者主动要办法时，协助她准备一句表达需要或界限的话；她提出演练时，模拟一轮，并且一次只反馈一个调整点。 | 不采用成人职场、约会和谈判场景；不在她还想倾诉时自动生成沟通脚本；欺凌和胁迫不能按普通争执处理。 |
| [ivangdavila / psychologist](https://clawhub.ai/ivangdavila/skills/psychologist) | 先确认感受，不拿别人的经历作比较；用开放问题代替盘问。 | 不采用“心理学家”身份设定，也不把平台上的“循证”描述当成临床资质证明；不让 AI 充当未成年人的咨询师。 |
| [MetcalfSolutions / Satori](https://github.com/MetcalfSolutions/Satori/blob/main/SKILL.md)；[临床流程](https://github.com/MetcalfSolutions/Satori/blob/main/references/clinical-spine.md)；[语气指南](https://github.com/MetcalfSolutions/Satori/blob/main/references/tone-and-voice.md) | 从具体经历而非泛泛安慰出发；情绪很重时先留在倾听；猜测允许对方纠正；回应长度随故事内容变化；只在画面能照亮具体经历时使用比喻。 | 不采用每轮都必须产生洞见或行动的要求、对人格与旧创伤的主动解释、长期心理记忆、哲学框架或“智慧伙伴”人格。该 skill 的自述不等于临床审核。 |
| [heartpunk / motivational-interviewing](https://github.com/heartpunk/motivational-interviewing-skill/blob/main/motivational-interviewing/skills/motivational-interviewing/SKILL.md)；[参考文献](https://github.com/heartpunk/motivational-interviewing-skill/blob/main/motivational-interviewing/skills/motivational-interviewing/resources/references.md) | 对矛盾心情作可纠正的双面复述；不争辩、不催决定；在她明确想推进时使用一个开放问题，保留自主权。 | 不采用每轮必须以问题结尾、数字量尺和决策平衡表作为常规回应；不把其引用的动机式访谈研究或语料分析当作本草案有效性的证明。 |

另查看了 [jhillin8 / relationship-skills](https://clawdir.com/skill/relationship-skills/)：其倾听与表达需要的做法与上面的技能重合，但“所有数据只留本机”的保证无法由 skill 文本实现，因此没有采用它作为主要底本。

短时间线、双向心情箭头和学习流程图是为本草案新增的表达方式，不是外部 skill 经验证的治疗技术。它们只整理当事人已说出的信息，不能替代倾听、临床评估或现实支持。

## 面向青少年与LGBT话题的独立核验

2026-10-05 重新核对了下列机构原始页面的正文，但当前环境没有可信的中国大陆网络测试点，**不能证明这些页面在大陆可访问**。因此运行中的 skill 不依赖这些外部页面，而使用 [lgbt-decision-standards.md](lgbt-decision-standards.md) 的中文判断标准；此处只保留出处名称用于审阅，不把境外求助入口交给青少年作为当地资源。

- The Trevor Project，《The Coming Out Handbook》：探索身份不必立即确定标签，也没有必须出柜的时间表；披露对象和安全由年轻人自己判断。
- The Trevor Project，《A Guide to Being an Ally to Transgender and Nonbinary Young People》：尊重自选称呼，未经允许不披露他人的身份，避免侵入性提问。
- American Academy of Child and Adolescent Psychiatry（AACAP），《Conversion Therapy》（2018）：不把性取向、性别认同或性别表达视为需要被改变的病理状态，不采用以改变身份为目标的所谓“转化治疗”。
- [NIMH 儿童与青少年心理健康说明](https://www.nimh.nih.gov/health/topics/child-and-adolescent-mental-health)：困扰持续并影响生活时连接专业帮助。

以上来源提供设计依据，不构成对此草案的临床审核、疗效评估或面向未成年人的安全认证。本草案保持未安装状态。

## 青少年心理学资料的新增借鉴（2026-10-05）

详见 [adolescent-psychology-foundations.md](adolescent-psychology-foundations.md)。这次优先采用机构原始资料，而不把第三方 skill 的自述当作专业证据。

| 来源 | 写入草案的具体判断 | 适用边界 |
|---|---|---|
| [WHO《青少年精神卫生》](https://www.who.int/zh/news-room/fact-sheets/detail/adolescent-mental-health)（2025） | 在讨论故事时留意她已提及的家庭、同伴、学校、网络、欺凌与歧视；教学中区分发展背景和个人结论。 | WHO 描述的是人群和环境因素，不能据此解释某个青少年的病因。 |
| [UNICEF 中国站《14–18 岁：开启关于心理健康的对话》](https://www.unicef.cn/mental-health/conversation-starters-14-18-years) | 让她保留谈话主动权；用开放、澄清式对话；不忽视网络经历和归属感。 | 原文面向照护者，不能直接证明 AI 的陪伴能力。 |
| [WHO 青少年心理健康促进指南](https://www.who.int/publications/b/55043)与[中文执行摘要](https://iris.who.int/bitstream/handle/10665/341140/9789240023826-chi.pdf) | 学习路径增加社会情感技能与环境因素；只用虚构案例练习。 | 指南面向政策与项目实施，不能当作本 skill 疗效证据。 |
| [UNICEF 中国站同伴支持项目](https://www.unicef.cn/stories/silence-sharing-power-peer-support) | 教会“观察、倾听、转介”的边界，不让未成年人承担治疗同学的责任。 | 这是项目报道，不等于对任意同伴支持方式的疗效验证。 |
| [NIMH 儿童与青少年心理健康说明](https://www.nimh.nih.gov/health/topics/child-and-adolescent-mental-health) | 当困扰持续数周并影响生活时，推动现实专业评估；眼前危险不等数周。 | 美国求助电话和服务路径不直接移植到中国。 |
| [国家卫健委“五健”行动计划解读](https://www.nhc.gov.cn/fys/c100077/202512/156aee28a1f543f1a3301ab92580a48b.shtml) | 将学校、家庭与医疗机构放在现实支持网络中。 | 官网正文抓取受限，当前仅依据官方搜索摘录；具体当地服务仍须单独核验。 |
| [WHO、UNICEF、UNESCO《Teaching with Care》](https://www.who.int/publications/i/item/9789240124912)（2026）与[UNICEF AI 伴侣政策简报](https://www.unicef.org/documents/when-ai-becomes-friend-child-rights-risks)（2026） | 支持者不做诊断，AI 不塑造排他关系；加强隐私与现实连接。 | 前者面向教师，后者面向政策与服务提供者，均未审查本 skill。 |

上表中的外部页面未从中国大陆网络测试点独立核验可达性。草案在运行时读取本地中文判断标准，不以打开网页作为对话条件。

## 自愿的小方法与收尾节奏（2026-10-05）

[UNICEF 中国站《通过五个技巧，开启围绕心理健康的对话》](https://www.unicef.cn/mental-health/five-tips-how-start-talking-about-mental-health)将写日记作为难以开口时表达感受的一个选项；[UNICEF《3 ways you can help your teen express emotions》](https://www.unicef.org/parenting/mental-health/3-ways-help-teens-express-emotions)强调先共情，也提到音乐、画画等非语言表达。草案只借鉴“提供表达入口”的做法：先听她的具体经历，收尾时仅在她想缓解压力或谈话自然转向下一步时，轻轻说明 AI 能协助什么；她选择后才展开一项。上述资料不证明写日记对她个人有效，也不证明 AI 能治疗焦虑。

## 非联合国资料的补充与反证（2026-10-05）

- [AAP 青少年沟通材料](https://www.healthychildren.org/English/family-life/family-dynamics/communication-discipline/Pages/How-to-Communicate-with-a-Teenager.aspx)提醒家长先听、不灾难化，也不要因共情而立即谴责故事里的另一个人。草案借鉴的是准确回应和保留未知，不把家长角色交给 AI。
- [AAP 面向 12–18 岁的压力材料](https://www.healthychildren.org/English/healthy-living/emotional-wellness/Building-Resilience/Pages/For-Teens-Creating-Your-Personal-Stress-Management-Plan.aspx)与[AACAP 青少年压力说明](https://www.aacap.org/AACAP/Families_and_Youth/Facts_for_Families/FFF-Guide/Helping-Teenagers-With-Stress-066.aspx)都列出写作、创作、听音乐、与可信的人交谈等方式。草案保留“她自愿选一项”的流程，不照搬完整计划，也不承诺效果。
- [AACAP 2026 年 AI 聊天机器人家长说明](https://aacap.org/AACAP/AACAP/Families_and_Youth/Facts_for_Families/FFF-Guide/AI_Chatbots-148.aspx)对儿童使用 AI 伴侣提出强烈警示：可能削弱现实交往，焦虑或抑郁的青少年更需谨慎。[AACAP 2026 年政策声明](https://aacap.org/AACAP/Policy_Statements/2026/AI_Role_Delivery_Child_Adolescent_Mental_Health_Care.aspx)要求用于儿童青少年心理健康服务的 AI 接受严谨测试与隐私保护。**本草案没有完成这些验证**；因此主文件新增“AI 对话挤占现实关系与生活”的识别及退出分支。AACAP 的材料不能被曲解为对这个 skill 的认可。
- [教育部《中小学心理健康教育指导纲要》](https://www.moe.gov.cn/srcsite/A06/s3325/201212/t20121211_145679.html)支持尊重学生、个别差异和学生主体性；[国家卫健委“五健”行动计划](https://www.nhc.gov.cn/fys/c100078/202512/9c3da4badfb34026b5fabbf5853105ee.shtml)把学校、家庭、医疗机构和隐私保护纳入现实服务体系。两者均不能证明某地已有具体可用服务，也不构成 AI 对话的临床规范。

各来源的使用位置、适用人群和限制列在 [adolescent-psychology-foundations.md](adolescent-psychology-foundations.md)。境外页面仍未经中国大陆网络独立验证，运行时只用本地规则。

## “看见委屈与伤害”成为优先动作（2026-10-05）

前版虽然要求对欺凌、胁迫和虐待承认伤害，但在普通人际故事中更强调梳理关系、区分事实与猜测，容易过早进入“客观分析”。本版把优先动作改为：找出她描述的受伤片段，回应那件事怎样碰到了她的信任、期待或边界；之后才讨论对方动机和下一步。所依据的沟通原则包括[AAP《How to Communicate With and Listen to Your Teen》](https://www.healthychildren.org/English/family-life/family-dynamics/communication-discipline/Pages/How-to-Communicate-with-a-Teenager.aspx)的先倾听、不灾难化与不因过度同情而替孩子裁决同伴关系，以及[UNICEF 的共情在先材料](https://www.unicef.org/parenting/mental-health/3-ways-help-teens-express-emotions)。这些材料面向家长；移用于 AI 对话是设计推论，未经临床验证。

“她感到被伤害”与“我们已经知道对方动机”是不同判断。草案要求承认前者，不凭单方故事断言后者；遇到明确的羞辱、泄密、欺凌或胁迫，也不以保持中立为由淡化发生的行为。示例见 [conversation-examples.md](conversation-examples.md)。

## 用户提供文章的逐篇审阅（2026-10-05）

- [最初两篇文章评估](two-articles-assessment.md)：区分家人期待与孩子意愿、透明说明 AI 身份、尊重不谈；排除“天生高敏感导致心理问题”、单因解释和“不接受咨询就服药”的跳跃。
- [后续四篇文章评估](additional-articles-assessment.md)：保留失落发生时先倾听、外在开朗不能否定当事人痛苦、取得谈话许可与尊重沉默；排除“微笑抑郁”诊断化、无出处统计、脑机制断言、早年创伤推断，以及把“不求不助”当作未成年人安全的绝对规则。

这六篇是作者观点和叙述素材。网页可达性、作者资质与个案效果的核验状态在对应评估文件中说明；主文件的风险边界优先依据机构原始资料。本次增补没有使草案获得临床评估或适龄安全认证，也没有改变未安装状态。

## 《被讨厌的勇气》作为学习资料（2026-10-05）

用户提供的笔记依据岸见一郎、古贺史健著、渠海霞译的中文 EPUB，以“第几夜＋小节名”定位。原始笔记保留在工作区的 `source-materials/books/被讨厌的勇气-中心思想.md`，不随 skill 打包。供运行时读取的[精简学习参考](adler-book-learning.md)只在使用者主动提出学习本书或阿德勒观点时启用；它把书中观点、虚构案例和适用边界分开。

尤其没有把书中对创伤的否认、对拒学或恐惧的目的解释写成个人判断。[NIMH 关于创伤与 PTSD 的说明](https://www.nimh.nih.gov/health/topics/post-traumatic-stress-disorder-ptsd)确认创伤经历可能有持续影响，也说明影响因人而异；[SAMHSA 创伤知情原则](https://www.samhsa.gov/mental-health/trauma-violence/trauma-informed-approaches-programs)强调安全和当事人的声音与选择。[UNICEF 青少年工作指南](https://www.unicef.org/adolescentkit/reports/guide-ten-key-approaches-working-adolescents)同时支持尊重青少年的表达意愿与受威胁时的保护行动。以上资料没有审核或认可本 skill，境外页面的中国大陆可达性未独立实测。

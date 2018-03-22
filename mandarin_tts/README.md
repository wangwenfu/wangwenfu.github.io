**Syllable-based End-to-end Text-to-speech Synthesis for Mandarin Chinese**   
Wenfu Wang, Bo Xu, Meng Meng

## Abstract
The complex pipeline design of a conventional text-to-speech (TTS) system requires much significant domain expertise and human engineering. Building such a system is nontrivial. This paper presents a neural approach towards end-to-end Mandarin Chinese text-to-speech synthesis based on syllables. We propose an improved model based on Google's Tacotron to cope with this challenging task. Our model can synthesize speech directly from Mandarin tonal syllables (a.k.a. pinyin), achieving a mean opinion score (MOS) of 3.81 in naturalness. We also present a multi-speaker variant which synthesizes speech with each speaker's timbre and speaking style well retained with only some simple modifications to the decoder. Furthermore, speaker adaption is investigated based on the trained multi-speaker model. Experiments show it can transfer to a new voice producing acceptable quality using as little as 10 minutes of data, making it a promising way to quickly build a TTS system.

## Audio Samples
### 1. Mandarin Chinese TTS
#### 1.1 Our model *vs* Tacotron

test01: **"好好学习，天天向上。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Tacotron:&#160;&#160;&#160;</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test01_tacotron.wav" /></audio></td>
  </tr>
</table>
 
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test01_ours.wav" /></audio></td>
  </tr>
</table>

test02: **"红红火火，和和美美，团团圆圆。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Tacotron:&#160;&#160;&#160;</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test02_tacotron.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test02_ours.wav" /></audio></td>
  </tr>
</table>

#### 1.2 Some other samples

test03: **"北京时间十六日晚十点，多国科学家宣布探测到中子星引力波事件，引发广泛关注。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news06.wav" /></audio></td>
  </tr>
</table>

test04: **"此次引力波探测的一大优点是不仅能“听到”，还能“看到”。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news05.wav" /></audio></td>
  </tr>
</table>

test05: **"如果我们今天没有解决方案，不等于我们的孩子没有解决方案。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news07.wav" /></audio></td>
  </tr>
</table>

test06: **"马云又为年轻人打call：相信年轻人，不要担忧未来。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Our model:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news08.wav" /></audio></td>
  </tr>
</table>

### 2. Multi-speaker TTS

test01: **"刘国梁在微博中称，我认为中国体育改革势在必行。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 001:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk001.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 012:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk012.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 091:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk091.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 112:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk112.wav" /></audio></td>
  </tr>
</table>

test02: **"他曾培养出多名世界冠军。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 001:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk001.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 012:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk012.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 091:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk091.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker 112:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk112.wav" /></audio></td>
  </tr>
</table>

### 3. Speaker Adaption

test01: **"端到端语音合成。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test02_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test02_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test02_adpt_10min.wav" /></audio></td>
  </tr>
</table>

test02: **"中国拟放开汽车、电子等领域外资股比限制。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/news03_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/news03_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/news03_adpt_10min.wav" /></audio></td>
  </tr>
</table>

test03: **"金州勇士队四比一克里夫兰骑士队，夺取总冠军。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test13_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test13_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/adaption/test13_adpt_10min.wav" /></audio></td>
  </tr>
</table>

## Appendix
### 1. Test scripts for MOS
test01 端到端语音合成。   
test02 生成式对抗网络。   
test03 好好学习，天天向上。   
test04 球星科比布莱恩特于去年退役。   
test05 金州勇士队四比一克里夫兰骑士队，夺取总冠军。   
test06 当地时间六月一日下午，特朗普在白宫宣布美国将推出巴黎气候协议。   
test07 北京高考文科状元，清华还是北大没想好，现在最想脱单。   
test08 中国拟放开汽车电子等领域外资股比限制。   
test09 刘国梁在微博中称，我认为中国体育改革势在必行。   
test10 北京时间十六日晚十点，多国科学家宣布探测到中子星引力波事件，引发广泛关注。   
test11 此次引力波探测的一大优点是不仅能听到，还能看到。   
test12 北京城市副中心与河北雄安新区是北京发展的新“两翼”。   
test13 北京市代市长陈吉宁表示，“两翼”间非竞争关系。   
test14 他强调，做好历史文化名城保护和城市特色风貌塑造。   
test15 “一带一路”倡议是中国对于解决国际问题贡献的中国智慧和中国方案。   
test16 而中巴经济走廊的建设也彰显着中国的影响力。   
test17 这些突出的建设成绩，让巴基斯坦百姓真切感受到正在发生的、和可以预期的生活改善。   
test18 2017年以来，平均每月有近6000名巴基斯坦人申请签证前往中国。   
test19 其中上海、北京、广州成为访问频率最高的中国城市。   
test20 中国最近五年正在为经济全球化做出越来越多的贡献。   
test21 又为何能够在过去五年强势增长？   
test22 中国人“更爱储蓄”的旧有形象正在改变。   
test23 去年中国大陆游客境外消费总额连续第五年全球居首。   
test24 第一，抓改革，释放发展活力。   
test25 我们的一些优秀作品不仅在国内叫得响、传得开。   
test26 我们的产品在世界上也开始建立品牌，赢得了市场份额。   
test27 我们大力实施精品战略，鼓励精品、鼓励原创。   
test28 对陕西人而言，似乎没有哪一种食物比得上一碗面。   
test29 一碗拉条子，没有花里胡哨的讲究，只一个字，爽。   
test30 有人将兰建波拉面的镜头拍下来，发在网上，迅速引起关注。   
test31 网友将他称为西安“拉面哥”。   
test32 谁想学，可以来找我，我免费传授技术。   
test33 每天只卖100碗左右，每一碗面都是精品。   
test34 没想到有一天，我也会向你们推荐曾国藩。   
test35 他认为，应该集中力量攻下长沙和安庆这样的重镇。   
test36 在现阶段，这简单的几个字给了我很大的力量。   
test37 现在的很多年轻人仍有这样的刻板印象。   
test38 很多愚蠢的决定都是出于好意。   
test39 普京称阿里巴巴“是一家伟大的公司”。   
test40 马云此前与普京在圣彼得堡经济论坛等场合有过两次会面。   
test41 议题涉及单边主义、核危机、地缘政治等重大国际命题。   
test42 如果我们今天没有解决方案，不等于我们的孩子没有解决方案。   
test43 昨天，北方出现入秋以来首轮大雾天气。   
test44 今天大雾持续，还会带来低能见度天气。   
test45 不过中东部地区晴多雨少的天气格局对于秋收秋种十分有利。   
test46 气象专家建议农民朋友们抓紧有利时机进行抢收抢种。   
test47 在以前，车子都是不会主动礼让行人的。   
test48 学员可在充分熟悉驾驶技能之后再报考。   
test49 酒的价格不在于贵，太贵的酒不一定卖得好。   
test50 为方便市民游客欣赏秋韵，杭州15条道路白天不扫落叶。   

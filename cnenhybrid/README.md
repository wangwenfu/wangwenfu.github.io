**Towards End-to-end Text-to-speech for Chinese-English Hybrid and Multi-speaker Synthesis**   
Wenfu Wang, Meng Meng, Peng Gao, Bo Xu

## Abstract


## Audio Samples
### 1. Chinese-English Hybrid TTS
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
  <td style="border: none; vertical-align: middle;">Speaker001:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk001.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker012:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk012.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker091:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk091.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker112:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/news04_spk112.wav" /></audio></td>
  </tr>
</table>

test02: **"他曾培养出多名世界冠军。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker001:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk001.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker012:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk012.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker091:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk091.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">Speaker112:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/multispk/test06_spk112.wav" /></audio></td>
  </tr>
</table>

### 3. Speaker Adaption

test01: **"端到端语音合成。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test02_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test02_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test02_adpt_10min.wav" /></audio></td>
  </tr>
</table>

test02: **"中国拟放开汽车、电子等领域外资股比限制。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news03_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news03_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/news03_adpt_10min.wav" /></audio></td>
  </tr>
</table>

test03: **"金州勇士队四比一克里夫兰骑士队，夺取总冠军。"**
<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">25 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test13_adpt_25min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">18 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test13_adpt_18min.wav" /></audio></td>
  </tr>
</table>

<table style="border: none;">
  <tr>
  <td style="border: none; vertical-align: middle;">10 min:</td>
  <td style="border: none; vertical-align: middle;"><audio controls=""><source src="demos/test13_adpt_10min.wav" /></audio></td>
  </tr>
</table>

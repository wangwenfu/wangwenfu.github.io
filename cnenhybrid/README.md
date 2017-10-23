**Towards End-to-end Text-to-speech for Chinese-English Hybrid and Multi-speaker Synthesis**   
Wenfu Wang, Meng Meng, Peng Gao, Bo Xu

## Abstract
The complex pipeline design of a conventional Text-to-speech (TTS) system requires much significant domain expertise and human engineering. Building an engine supporting multi-language and multi-speaker is nontrivial. This paper presents an approach towards end-to-end Chinese-English hybrid text-to-speech synthesis. We propose an improved model based on Google's Tacotron to cope with this challenging task. Our model can synthesize speech directly from Chinese pinyins and English phonemes, achieving a mean opinion score (MOS) of 3.87 in naturalness for Chinese synthesis. We also present a multi-speaker variant which synthesizes speech with each speaker's timbre and speaking style well retained with only some simple modifications to the decoder. Furthermore, speaker adaption is investigated based on the trained multi-speaker model. Experiments show it can transfer to a new voice producing acceptable quality using as little as 10 minutes of data, making it a promising way to quickly build a TTS system.

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

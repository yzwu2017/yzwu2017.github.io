---

layout:     post
title:      "Notes for Reverberation"
date:       2021-12-07 16:45:00
author:     "Yuzhong Wu"
header-img: "img/color_strip/deep-blue.jpg"
comments: true
---



**Add Reverberation Using SoX**

<p>To add reverberation, use the following command: </p>
```shell
sox input.wav output.wav reverb 50 50 100 100 0 0
```

<br />

<p>Usage</p>
```sh
sox input.wav output.wav reverb [reverberance_% 0~100] [hf_damping_% 0~100] [room_scale_% 0~100] [stere_depth_% 0~100] [pre_delay_ms 0~500] [wet_gain_db -10~10]
```

<p>The meaning of the parameters</p>
<ul>
	<li>reverberance (混响大小): how long it takes for the reverb sound to die. </li>
	<li>HF-damping (高频阻尼): Damping makes high frequencies of reverb die faster.</li>
	<li>room-scale (房间大小): A larger value means a larger room. </li>
	<li>stere_depth (立体声深度): -</li>
	<li>pre-delay (早反射声的时间，单位是ms): the amount of time between the original sound and the audible onset of early reflections. </li>
    <li>wet-gain (湿声增益): a dry signal means the original signal; a wet signal means the resulted signal.  </li>
</ul>
<br />
Reference: http://sox.sourceforge.net/sox.html


<br />
<br />

**Readings**

Breaking down the behavior of reverb: https://www.redsharknews.com/audio/item/4150-breaking-down-the-behaviour-of-reverb

Handbook for acoustic ecology - reverberation: http://www.sfu.ca/sonic-studio-webdav/cmns/Handbook%20Tutorial/Reverberation.html




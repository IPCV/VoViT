---
layout: page
title: VoViT
subtitle: Low Latency Graph-based Audio-Visual Voice Separation
---

<div class="lead mb-0" align="justify" style="padding-bottom: 1em">
The VoViT model consist of TODO 
</div>

![VoViT](../img/model.png)  

## Latency   

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#93a1a1;border-spacing:0;margin:0px auto;}
.tg td{background-color:#fdf6e3;border-color:#93a1a1;border-style:solid;border-width:0px;color:#002b36;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#657b83;border-color:#93a1a1;border-style:solid;border-width:0px;color:#fdf6e3;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky"></th>
    <th class="tg-c3ow">Preprocessing</th>
    <th class="tg-c3ow" colspan="2">Inference</th>
    <th class="tg-c3ow">Preprocessing + Inference</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow">Graph Network</td>
    <td class="tg-c3ow">Whole model</td>
    <td class="tg-c3ow"></td>
  </tr>
  <tr>
    <td class="tg-0pky">VoViT-s1</td>
    <td class="tg-c3ow">17.95</td>
    <td class="tg-c3ow">4.50</td>
    <td class="tg-c3ow">52.21</td>
    <td class="tg-c3ow">82.18</td>
  </tr>
  <tr>
    <td class="tg-0pky">VoViT</td>
    <td class="tg-c3ow">17.95</td>
    <td class="tg-c3ow">4.55</td>
    <td class="tg-c3ow">57.45</td>
    <td class="tg-c3ow">93.31</td>
  </tr>
  <tr>
    <td class="tg-0pky">VoViT-s1 fp16</td>
    <td class="tg-c3ow">10.94</td>
    <td class="tg-c3ow">2.88</td>
    <td class="tg-c3ow">30.47</td>
    <td class="tg-c3ow">52.43</td>
  </tr>
  <tr>
    <td class="tg-0pky">VoViT fp16</td>
    <td class="tg-c3ow">10.94</td>
    <td class="tg-c3ow">2.86</td>
    <td class="tg-c3ow">34.18</td>
    <td class="tg-c3ow">46.14</td>
  </tr>
</tbody>
</table>  


Latency estimation for the different variants of VoViT. Average of 10 runs, batch size 100. Device: Nvidia RTX 3090. GPU utilization >98%, memory on demand. Two forward passed done to warm up. 
Timing corresponds to ms to process 10s of audio

**Note: Pytorch version is no longer supporting complex32 dtype in pytorch 1.11**

<div class="lead mb-0" align="justify" style="padding-bottom: 1em">
TODO
</div>

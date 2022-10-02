---
title: "Applying Objective Quality Metrics to Video&#8209;Codec Comparisons: Choosing the Best Metric for Subjective Quality Estimation"
permalink: /best_metric_Subjective_QA
features:
  - "Comparison of SSIM, MS-SSIM, PSNR, NIQE, VQM and VMAF"
  - "<b>39</b> versions of H.264, H.265, AV1, VP9, and other codecs at three bitrates"
  - "<b>789</b> encoded videos and <b>320&#x202F;294</b> subjective scores"
  - "Comparison of different YUV summations"
---


### A.&#x202F;Antsiferova, A.&#x202F;Yakovenko, N.&#x202F;Safonov, D.&#x202F;Kulikov, A.&#x202F;Gushin and D.&#x202F;Vatolin

Contact&nbsp;us:

* <aantsiferova@graphics.cs.msu.ru>
* <video@compression.ru>

## Abstract

Quality assessment is essential to&nbsp;creating and comparing video compression algorithms. Despite the development&nbsp;of many new quality assessment methods, well-known and generally accepted codecs comparisons mainly employ classical methods such&nbsp;as PSNR, SSIM, and VMAF. These methods have different variations: temporal pooling techniques, color component summations and versions. In&nbsp;this&nbsp;paper, we present comparison results&nbsp;for generally accepted video quality metrics to&nbsp;determine which ones are most relevant&nbsp;to video codecs comparisons. For&nbsp;evaluation we used videos compressed&nbsp;by codecs of different standards&nbsp;at three bitrates, and subjective scores were collected&nbsp;for these videos. Evaluation dataset consists&nbsp;of 789 encoded streams and 320&#x202F;294 subjective scores. VMAF calculated&nbsp;for all Y, U, V color spaced showed the best correlation with subjective quality, and we also showed that the&nbsp;usage&nbsp;of smaller weighting coefficients&nbsp;for U and V components leads&nbsp;to a&nbsp;better correlation with subjective quality.

<!-- Add Download Full Text button-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<div>
<button class="download-button" role="button" onauxclick="window.open('http://ceur-ws.org/Vol-3027/paper19.pdf')" onclick="window.open('http://ceur-ws.org/Vol-3027/paper19.pdf')"> <!-- Insert link here-->
    <i class="fa fa-download"></i>
    Download Full Text
</button>
<p class="download-button-caption">(PDF, 3.9 MB)</p>  <!-- Insert correct filesize here-->
</div>

## Key Features

* Comparison of SSIM, MS-SSIM, PSNR&nbsp;(avg.&nbsp;mse,&nbsp;log), NIQE, VQM and VMAF&nbsp;(v061&#8209;v063,&nbsp;v061_neg)
* **39** versions of H.264, H.265, AV1, VP9, and other codecs at three bitrates
* **789** encoded videos and **320&#x202F;294** subjective scores
* Comparison of YUV summations: YUV&#x202F;1:1:1, YUV&#x202F;2:1:1, YUV&#x202F;4:1:1, YUV&#x202F;6:1:1, YUV&#x202F;8:1:1 and YUV&#x202F;10:1:1

## Data Collection for Evaluating Video&nbsp;Quality&nbsp;Assessment Algorithms

To analyze the relevance of quality metrics to codec comparisons, we collected a special data set that includes video sequences and subjective scores. We made our selection from a pool of more than 18,000 open source clips with high bitrate after analyzing more than five million source videos from the Vimeo website. A description of the video selection method appears in [2].The resulting video data sets for subjective assessments are called CC-2018, CC-2019, CC-2020, and UGC-2020, each data set is available by request from its associated codec comparison project page [1].

Table below summarizes the data sets, which the 2018–2020 MSU codec comparisons used for subjective evaluation.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-baqh"><span style="font-weight:bold">VIdeo</span><br><span style="font-weight:bold">dataset</span></th>
    <th class="tg-amwm">Number of <br>codecs</th>
    <th class="tg-amwm">Number of <br>test videos</th>
    <th class="tg-amwm">Number of <br>encoded streams</th>
    <th class="tg-amwm">Number of <br>responses</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-amwm">CC-2018</td>
    <td class="tg-baqh">10</td>
    <td class="tg-baqh">5</td>
    <td class="tg-baqh">150</td>
    <td class="tg-baqh">22542</td>
  </tr>
  <tr>
    <td class="tg-amwm">CC-2019</td>
    <td class="tg-baqh">11</td>
    <td class="tg-baqh">5</td>
    <td class="tg-baqh">165</td>
    <td class="tg-baqh">25784</td>
  </tr>
  <tr>
    <td class="tg-amwm">CC-2020</td>
    <td class="tg-baqh">11</td>
    <td class="tg-baqh">8</td>
    <td class="tg-baqh">264</td>
    <td class="tg-baqh">236736</td>
  </tr>
  <tr>
    <td class="tg-amwm">UGC-2020</td>
    <td class="tg-baqh">7</td>
    <td class="tg-baqh">10</td>
    <td class="tg-baqh">210</td>
    <td class="tg-baqh">35232</td>
  </tr>
  <tr>
    <td class="tg-amwm">Total</td>
    <td class="tg-baqh">39</td>
    <td class="tg-baqh">28</td>
    <td class="tg-baqh">789</td>
    <td class="tg-baqh">320294</td>
  </tr>
</tbody>
</table>

The subjective assessment involved pairwise comparisons using the Subjectify.us platform, each pair of videos received at least 10 responses from participants.



## Comparison of YUV Summations

Table below shows the best options for summing the components of different metrics.
Some options have almost identical correlation; the table separates them by commas.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Metric&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Best YUV Summing</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">VMAF 0.6.1<br>VMAF 0.6.2<br>VMAF 0.6.3<br>VMAF 0.6.1 phone<br>VMAF 0.6.1 neg&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8:1:1, 10:1:1, 6:1:1<br>VMAF 0.6.1 neg phone<br>VMAF 0.6.1 4K<br>VMAF 0.6.2 phone<br>VMAF 0.6.3 phone</td>
  </tr>
  <tr>
    <td class="tg-0pky">PSNR avg. MSE&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6:1:1, 4:1:1<br>PSNR avg. log</td>
  </tr>
  <tr>
    <td class="tg-0pky">SSIM&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; No significant difference between summing methods&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0pky">MS-SSIM&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Y (only luma component), 10:1:1, 6:1:1, 8:1:1</td>
  </tr>
</tbody>
</table>


## Overall Ranking of Metrics

Because we conducted a separate subjective comparison of the videos for each year, we had to obtain for every metric an overall correlation across the entire data set. For each metric, our approach applied the Fisher z-transform to all correlations coefficients calculated on individual video sequences and used the resulting values to calculate the weighted mean and confidence interval, with the weights proportional to the number of distortions. We determined the final correlations using the inverse transformation [3].

Below is the overall ranking of metrics with best summations only.

<img src="/assets/img/papers/Applying _Objective_Quality_Metrics_to_Video-Codec_Comparisons/Fig.3.png">

## Contact us

For questions and propositions, please contact us: <aantsiferova@graphics.cs.msu.ru> and <video@compression.ru>

## See also 
* [MSU Video Codecs Comparisons](http://compression.ru/video/codec_comparison/index_en.html)
* [Subjectify.us](http://www.subjectify.us/)
* [Hacking VMAF and VMAF NEG: Vulnerability to Different Preprocessing Methods](https://videoprocessing.github.io/hacking-vmaf-and-vmaf-neg)

## References <!-- Other papers that were mentioned in the main part of the page -->

1.  Msu video codecs comparisons, n.d. URL: http://compression.ru/video/codec_comparison/index_en.html.

2.  A.&#x202F;V.&#x202F;Zvezdakova, D.&#x202F;L.&#x202F;Kulikov, S.&#x202F;V.&#x202F;Zvezdakov, D.&#x202F;S.&#x202F;Vatolin, Bsq-rate: anewapproachfor video-codec performance comparison and drawbacks of current solutions, Programming and computer software 46 (2020) 183–194.

3.  D.&#x202F;M.&#x202F;Corey, W.&#x202F;P.&#x202F;Dunlap, M.&#x202F;J.&#x202F;Burke, Averaging correlations: Expected values and bias in combined pearson rs and fisher’s z transformations, The Journal of General Psychol- ogy 125 (1998) 245–261. URL: https://doi.org/10.1080/00221309809595548. doi:10.1080/ 00221309809595548. arXiv:https://doi.org/10.1080/00221309809595548.
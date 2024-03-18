---
title: A Hong Kong Sign Language Corpus Collected from Sign-interpreted TV News
---

## Introduction

We introduce _TVB-HKSL-News_, a large-vocabulary signer-dependent HKSL dataset for continuous sign language recognition (SLR) and sign language translation (SLT).
The dataset is collected from TVB News Report with Sign Language TV program.
It consists of 16.07 hours of sign videos of two signers with a vocabulary of 7,160 glosses for SLR and 2,850 Chinese characters (or 18K Chinese words) for SLT.

## Dataset Statistics

| name                                                  | Duration (h) | Samples | SLR vocab | SLR tokens | SLR #singletons | SLT vocab | SLT tokens | SLT #singletons | Duration (%) | Samples (%) | SLR Tokens (%) | SLT Tokens (%) |
| :---------------------------------------------------- | -----------: | :------ | :-------- | :--------- | :-------------- | :-------- | :--------- | --------------: | -----------: | ----------: | -------------: | -------------: |
| Overall                                               |        16.07 | 7,160   | 6,515     | 121,817    | 2,820           | 2,850     | 232,310    |             462 |          100 |         100 |            100 |            100 |
| <span style="white-space: nowrap;"> - Signer1 </span> |        11.66 | 5,350   | 5,476     | 88,788     | 2,362           | 2,695     | 173,027    |             450 |        72.59 |       74.72 |          72.89 |          74.48 |
| <span style="white-space: nowrap;"> - Signer2 </span> |         4.41 | 1,810   | 3,280     | 33,029     | 1,479           | 2,100     | 59,283     |             465 |        27.41 |       25.28 |          27.11 |          25.52 |
| Train                                                 |        14.71 | 6,516   | 6,515     | 111,204    | 2,925           | 2,816     | 212,108    |             466 |        91.53 |       91.01 |          91.29 |           91.3 |
| <span style="white-space: nowrap;"> - Signer1 </span> |        10.66 | 4,863   | 5,449     | 80,972     | 2,430           | 2,666     | 157,800    |             463 |        66.34 |       67.92 |          66.47 |          67.93 |
| <span style="white-space: nowrap;"> - Signer2 </span> |         4.05 | 1,653   | 3,234     | 30,232     | 1,520           | 2,069     | 54,308     |             468 |        25.18 |       23.09 |          24.82 |          23.38 |
| Dev                                                   |         0.67 | 322     | 1,091     | 5,222      | 471             | 1,279     | 10,003     |             395 |         4.18 |         4.5 |           4.29 |           4.31 |
| <span style="white-space: nowrap;"> - Signer1 </span> |         0.49 | 241     | 946       | 3,790      | 430             | 1,178     | 7,508      |             382 |         3.03 |        3.37 |           3.11 |           3.23 |
| <span style="white-space: nowrap;"> - Signer2 </span> |         0.18 | 81      | 503       | 1,432      | 264             | 710       | 2,495      |             286 |         1.15 |        1.13 |           1.18 |           1.07 |
| Test                                                  |         0.69 | 322     | 1,130     | 5,391      | 518             | 1,276     | 10,199     |             399 |         4.29 |         4.5 |           4.43 |           4.39 |
| <span style="white-space: nowrap;"> - Signer1 </span> |         0.52 | 246     | 1,001     | 4,026      | 503             | 1,195     | 7,719      |             410 |         3.21 |        3.44 |            3.3 |           3.32 |
| <span style="white-space: nowrap;"> - Signer2 </span> |         0.17 | 76      | 476       | 1,365      | 240             | 711       | 2,480      |             299 |         1.08 |        1.06 |           1.12 |           1.07 |

## Example Data

### Signer 1

<style>
    td {
        width: 300px;
    }

    th { 
        white-space: nowrap;
    }
</style>

<center>
<table style="word-break: normal; width: 100%">
  <thead>
    <tr>
      <th style="text-align: center">Video</th>
      <th style="text-align: center">SLR Glosses</th>
      <th style="text-align: center">SLT Characters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-07-13_024218-024346_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        肺 發炎 學校 分 一 房 最 多 四 學生 <br />
        (Lung Inflamed School One Room Maximum Four Students)
      </td>
      <td style="text-align: center">
        因應疫情將學生分流每個課室只安排最多四個學生 <br />
        (In response to the epidemic situation, students will be divided into
        groups and only a maximum of four students will be arranged in each
        classroom)
      </td>
    </tr>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-01-18_011156-011250_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        消息 說 他 香港 身份證 沒 但是 美國 護照 <br />
        (News Say His Hong Kong ID Not But US Passport)
      </td>
      <td style="text-align: center">
        消息指他無香港身份證但持有美國護照 <br />
        (It is reported that he does not have a Hong Kong identity card but
        holds a US passport)
      </td>
    </tr>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-01-28_026046-026152_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        兩 日 內 發生 一 二 三 有關 爆炸 爆炸 爆炸 情況 <br />
        (Two Days In Happen One Two Three Related Bomb Bomb Bomb Situation)
      </td>
      <td style="text-align: center">
        兩日內發生三宗涉及炸彈的案件 <br />
        (Three cases involving bombs in two days)
      </td>
    </tr>
  </tbody>
</table>
</center>

### Signer 2

<center>
<table style="word-break: normal; width: 100%">
  <thead>
    <tr>
      <th style="text-align: center">Video</th>
      <th style="text-align: center">SLR Glosses</th>
      <th style="text-align: center">SLT Characters</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-06-07_018080-018254_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        大埔 路 沙 田 坡 泥 傾瀉 因為 某些 地方 下雨 下雨 多 <br />
        (Tai Po Highway Sha Tin Slope Mud Pour Because Some Place Rain Rain
        Much)
      </td>
      <td style="text-align: center">
        大埔公路沙田段有護土牆塌下多處好似瀑布一樣 <br />
        (On the Sha Tin section of Tai Po Highway, the retaining wall has
        collapsed in many places like a waterfall)
      </td>
    </tr>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-01-21_001881-002184_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        國 衞生 健康 委員 說 湖 北 加 七 二 現在 全部 二 百 七 十 廣 東 一 四
        仍然 北京 五 上海 二 <br />
        (National Health Health Committee Say Hubei Add Seven Two Now Overall
        Two Hundred Seven Ten Guangdong One Four Still Beijing Five Shanghai
        Two)
      </td>
      <td style="text-align: center">
        國家衛健委公布湖北省新增 72 宗個案現時當地總數 270 宗廣東省維持 14
        宗首都北京 5 宗上海 2 宗 <br />
        (The National Health and Medical Commission announced that there were 72
        new cases in Hubei Province. The current local total is 270. Guangdong
        Province maintains 14 cases in the capital Beijing, 5 cases in Shanghai
        and 2 cases.)
      </td>
    </tr>
    <tr>
      <td style="text-align: center">
        <video width="200" controls>
          <source
            src="https://github.com/tvb-hksl-news/demo/raw/main/videos/2020-02-06_004876-005112_h264.mp4"
            type="video/mp4"
          />
        </video>
      </td>
      <td style="text-align: center">
        文 考試 日期 延後 學生 說 讀書 計劃 影響 混亂 某些 機構 說 語言 考試 這
        取消 變 不公平 <br />
        (Diploma Exam Date Postpone Student Say Study Plan Affect Disrupt Some
        Institution Say Language Exam Cancel Unfair)
      </td>
      <td style="text-align: center">
        文憑試延期有考生稱打亂溫習計劃有升學機構擔心一旦取消語文科口試會影響公平性
        <br />
        (HKDSE Postponement. Some candidates said it disrupted study plans. Some
        education institutions worried that cancellation of language oral
        examinations would affect fairness)
      </td>
    </tr>
  </tbody>
</table>
</center>

## Baseline Results

We have obtained baseline results on the _TVB-HKSL-News_ dataset with several popular SOTA SLR and SLT methods.

### Continuous Sign Language Recognition

| Method                 | Modality        | WER (%) Dev | WER (%) Test |
| :--------------------- | :-------------- | :---------- | :----------- |
| S3D [1,3]              | Keypoints       | 45.73       | 44.56        |
| S3D [1,3]              | Video           | 39.59       | 38.63        |
| VLT \[2\]              | Video           | 35.89       | 36.18        |
| C<sup>2</sup>SLR \[2\] | Video+Keypoints | 35.43       | 35.78        |
| TwoStream-SLR \[3\]    | Video+Keypoints | **34.52**   | **34.08**    |

<!--

| path                                  |   wer |
| :------------------------------------ | ----: |
| results/s3d_pose/dev/tvb_results.pkl  | 45.73 |
| results/s3d_rgb/dev/tvb_results.pkl   | 39.59 |
| results/vlt/dev_hyp.csv               | 35.89 |
| results/c2slr/dev_hyp.csv             | 35.43 |
| results/twostream/dev/tvb_results.pkl | 34.52 |

| path                                   |   wer |
| :------------------------------------- | ----: |
| results/s3d_pose/test/tvb_results.pkl  | 44.56 |
| results/s3d_rgb/test/tvb_results.pkl   | 38.63 |
| results/vlt/test_hyp.csv               | 36.18 |
| results/c2slr/test_hyp.csv             | 35.78 |
| results/twostream/test/tvb_results.pkl | 34.08 |

-->

### Sign Language Translation

| Method                                                          | Rouge (Dev) | BLEU-1 (Dev) | BLEU-2 (Dev) | BLEU-3 (Dev) | BLEU-4 (Dev) | Rouge (Test) | BLEU-1 (Test) | BLEU-2 (Test) | BLEU-3 (Test) | BLEU-4 (Test) |
| :-------------------------------------------------------------- | :---------- | :----------- | :----------- | :----------- | :----------- | :----------- | :------------ | :------------ | :------------ | :------------ |
| <span style="white-space: nowrap;">S3D (video) [1,3]</span>     | 18.64       | 21.98        | 15.17        | 11.18        | 8.79         | 21.61        | 25.39         | 18.59         | 14.57         | 12.10         |
| <span style="white-space: nowrap;">S3D (keypoints) [1,3]</span> | 15.65       | 18.18        | 11.58        | 8.09         | 6.22         | 16.42        | 19.93         | 13.72         | 10.41         | 8.48          |
| <span style="white-space: nowrap;">TwoStream-SLT \[3\]</span>   | **38.12**   | **43.22**    | **33.44**    | **26.04**    | **21.00**    | **39.80**    | **44.68**     | **35.27**     | **28.29**     | **23.58**     |

# Download

To download the dataset, please fill in the [request form](https://cse.hkust.edu.hk/tvb-hksl-news/docs/request-form-v2.pdf) and send to us via [email](mailto:mak@cse.ust.hk). After receiving your request, we will send you the download link and password to access the dataset.

# References

\[1\]: Saining Xie, Chen Sun, Jonathan Huang, Zhuowen Tu, and Kevin Murphy. 2018. Rethinking spatiotemporal feature learning: Speed-accuracy trade-offs in video classification. In ECCV, pages 305–321.

\[2\]: Ronglai Zuo and Brian Mak. 2022a. C<sup>2</sup>SLR: Consistency-enhanced continuous sign language recognition. In CVPR, pages 5131–5140.

\[3\]: Yutong Chen, Ronglai Zuo, Fangyun Wei, Yu Wu, Shujie Liu, and Brian Mak. 2022b. Two-stream network for sign language recognition and translation. In NeurIPS.

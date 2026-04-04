---
layout: index
title: "Beyond Segmentation: Structurally Informed Facade Parsing from Imperfect Images"
description1: Short Paper in Eurographics 2026
description2: Maciej Janicki<sup>1</sup>, Aleksander Plocharski<sup>1,2</sup> and Przemyslaw Musialski<sup>3</sup><br><sup>1</sup>Warsaw University of Technology, <sup>2</sup>Akces NCBR, <sup>3</sup>New Jersey Institute of Technology
button1_url: pdfs/beyond_segmentation.pdf
button1_text: Paper
button2_url: https://github.com/janickimaciej/beyond-segmentation
button2_text: Github
---

![Teaser](images/teaser.png)

# Abstract

Standard object detectors typically treat architectural elements independently, often resulting in facade parsings that lack the structural coherence required for downstream procedural reconstruction. We address this limitation by augmenting the YOLOv8 training objective with a custom lightweight alignment loss. This regularization encourages grid-consistent arrangements of bounding boxes during training, effectively injecting geometric priors without altering the standard inference pipeline. Experiments on the CMP dataset demonstrate that our method successfully improves structural regularity, correcting alignment errors caused by perspective and occlusion while maintaining a controllable trade-off with standard detection accuracy.

# Video

<div style="display: flex; justify-content: center;">
  <iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/Sk1JUOE0pIg"
    title="YouTube video player"
    frameborder="1"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>

# Models

Below are models for all the tested values of threshold T and weight W (see the paper for details).

<table>
  <tr>
    <th></th>
    <th colspan="3">Threshold T</th>
  </tr>
  <tr>
    <th>Weight W</th>
    <th>6</th>
    <th>7</th>
    <th>8</th>
    <th>9</th>
    <th>10</th>
    <th>11</th>
    <th>12</th>
  </tr>
  <tr>
    <td>0.1</td>
    <td><a href="https://drive.google.com/file/d/1iz-0TTGZ7KKmrTxS8fw158D5EDrSDSOX/view?usp=drive_link">T6_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/15xM9TbX2AqcDndkocTTFJJMkIbvMOCsV/view?usp=drive_link">T7_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1NGAVzB7rcuNl3HmkVC7hWatDMUyCpbLr/view?usp=drive_link">T8_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/10SSVxx4KTOMTEW9ksE7AjOpGwZ9sgS3L/view?usp=drive_link">T9_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1ElOUAzcVhulYgtt_DlJjEfDMdNyPfLAp/view?usp=drive_link">T10_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1b5-1wg_mX72x9pWIhpf5HoZDNkNu_JyR/view?usp=drive_link">T11_W0.1.pt</a></td>
    <td><a href="https://drive.google.com/file/d/17t1AUmIwKsWlfMh4dtNzXu20s9WdbxIA/view?usp=drive_link">T12_W0.1.pt</a></td>
  </tr>
  <tr>
    <td>0.25</td>
    <td><a href="https://drive.google.com/file/d/1qFpMcnpWR5LtQiH7j7C56dzc9qTo2pui/view?usp=drive_link">T6_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1i5nARhbIgj8auNoW6zmraOfCp6FlMV-n/view?usp=drive_link">T7_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1VnVJeo53Qvi6qVnGJr0hZ05p4NhJiOAm/view?usp=drive_link">T8_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1fFqIWtcNUUz2eN_2Pd11Cy_8kowU6TUc/view?usp=drive_link">T9_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1XRhC-mw3FsY12Psn7m6gcRW_nJaRWyUa/view?usp=drive_link">T10_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1DPrz2VwjaWZ7t5lwxPWDzG4cSyLBSzz_/view?usp=drive_link">T11_W0.25.pt</a></td>
    <td><a href="https://drive.google.com/file/d/19ZiY6KAh4IAaZ3lkpR4dtSno_RIVRe-1/view?usp=drive_link">T12_W0.25.pt</a></td>
  </tr>
  <tr>
    <td>0.5</td>
    <td><a href="https://drive.google.com/file/d/16N0EbNZTehX3zkQlbKOtIAc8_IVtON70/view?usp=drive_link">T6_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1fq2mm9Z1AhjYHbKeaUQsntRqLP_hf9yX/view?usp=drive_link">T7_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1PPENSOYNyUwNZYa7-Pw-9RdMOlvo14KN/view?usp=drive_link">T8_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/18tm-VjXtBzGVtBXJmgUStC9Gzune17a3/view?usp=drive_link">T9_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1weQHnf9zp4Qs30erOKrIpVAROhZNGI0_/view?usp=drive_link">T10_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1cu6mL8B-7njSvxaUs18O0Ls3Lt86_aOm/view?usp=drive_link">T11_W0.5.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1zCM4EkfGVx75DDawu3I9sWs8ORtd_PBN/view?usp=drive_link">T12_W0.5.pt</a></td>
  </tr>
  <tr>
    <td>0.75</td>
    <td><a href="https://drive.google.com/file/d/1uc_KUPJlsny54duQosTzSj2tDuLI8g9Z/view?usp=drive_link">T6_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1aVMmjnku_-Rj6EPewi7ZC4JttKt9LBi6/view?usp=drive_link">T7_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1xUtUxtEaNNv93kz1FqYhh6ITlkufWRv1/view?usp=drive_link">T8_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1kTO5RsIlLCDiGYxVKXI5HAjsC1oGfAvC/view?usp=drive_link">T9_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1eP8_oDiqLTGqmqumnyBSrDWq38gjS2Oy/view?usp=drive_link">T10_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1caI7q8DtcT4a7iy3JfhCoeH6mre4kzLx/view?usp=drive_link">T11_W0.75.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1x1TZAoa24ewK9dPZpwtYWUWWBSQzeqhC/view?usp=drive_link">T12_W0.75.pt</a></td>
  </tr>
  <tr>
    <td>1.0</td>
    <td><a href="https://drive.google.com/file/d/1mMaMPwT6nXKCrcvw2Jg7roTSk-KpPB58/view?usp=drive_link">T6_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1kcihptnDLBeCfjboWnmye3F3wewQLZLw/view?usp=drive_link">T7_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1zFJPurXgQAuZqA6FdThhQVxP8OUkOaQr/view?usp=drive_link">T8_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/170zfMaCoU2q21Sa5cEf5Sthax6L4tdLq/view?usp=drive_link">T9_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1LycspvEtsJkgMdyKCx1JWUZRUwI-_Cgt/view?usp=drive_link">T10_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1-d2r7Xma60j9Z_VKH3EIfMpQJGOzPWMb/view?usp=drive_link">T11_W1.0.pt</a></td>
    <td><a href="https://drive.google.com/file/d/1i6XM2pnLWMkekqxiuv5UKXQYO6BM9U0J/view?usp=drive_link">T12_W1.0.pt</a></td>
  </tr>
</table>

# BibTeX

```
TBD
```

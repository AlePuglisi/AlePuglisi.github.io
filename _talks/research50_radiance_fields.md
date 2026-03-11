---
title: "Radiance Fields Techniques - Review"
excerpt: "<img align='left' src='/images/research/ResearchRadianceFields.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**PhD Review - 20/01/2026** <br>
This presentation was a gentle introduction to **radiance fields** techniques for 3D reconstruction.
Firstly answering the basics of these algorithms: what is a radiance field, what is rendering, How to represent a 3D space, what metrics are used. Secondly, presenting the vanilla implementations of NeRF and 3DGS, and finally analyzing some extensions to improve reconstruction speed or broaden application domains (such as SLAM and underwater environments)."
collection: portfolio
---

**PhD Review** - 20/01/2026 | 3D Reconstruction - Deep Learning - Computer Graphics 
<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/Awesome-NeRFs-3DGS-underwater-robotics" class="btn btn--inverse">GitHub Resource</a>
</div> <br>

The presentation below was a PhD state-of-the-art review on 3D reconstruction with **radiance fields** techniques.
Although these topics are outside the scope of my PhD research, these algorithms are highly influential in the robotics community. Recognizing their importance, and as a result of my personal curiosity and fascination with these novel techniques, I provided a gentle introduction to the topic during one of my ongoing work update meetings.<br>
(This pdf version of the pptx slides is linked to the projects webpages and github repo, just click on the GitHub logo or the "World" logo)


<iframe src="/files/research/PhD_Review_Radiance_Fields.pdf" width="100%" height="800" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>


## Some Experimental 3D Gaussian Splat Reconstructions

Explore Some of my Gaussian Splat reconstruction obtained with [COLMAP SfM](https://colmap.github.io/) and [nerfstudio gsplat](https://docs.nerf.studio/nerfology/methods/splat.html). 
These models are obtained from few (200-300) phone images, extracted from video sequences. The purpose was mainly to experiment with the available radiance fields tools rather than obtaining optimal reconstruction results.  

<div style="display: flex; justify-content: center; align-items: flex-start; gap: 16px; margin: 1em 0;">

  <!-- Left column: GSplat (70%) -->
  <div style="width: 50%; display: flex; flex-direction: column;">
    <iframe 
      id="viewer" 
      allow="fullscreen; xr-spatial-tracking" 
      src="https://superspl.at/s?id=10e3843f"
      style="width: 100%; height: 400px; border: none; display: block;">
    </iframe>
    <p style="margin: 0.5em 0 0 0; font-size: 0.9em;">
      Fountain of the Three Graces - Place de la Comédie, Montpellier 
    </p>
  </div>

  <div style="width: 50%; display: flex; flex-direction: column;">
    <iframe 
      id="viewer" 
      allow="fullscreen; xr-spatial-tracking" 
      src="https://superspl.at/s?id=6bb6a719"
      style="width: 100%; height: 400px; border: none; display: block;">
    </iframe>
    <p style="margin: 0.5em 0 0 0; font-size: 0.9em;">
      Shared PhD Office at LIRMM - Montpellier
    </p>
  </div>

</div>
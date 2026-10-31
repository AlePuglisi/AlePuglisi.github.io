---
title: "GULP3R: Gaussian Underwater spLatting with semantic Perception for 3D Reconstruction. Creating Labeled 3D Maps from Camera Images"
excerpt: "<img align='left' src='/images/projects/ProjectGulp3r.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**MBARI-CoMPAS Lab Summer Internship - Completed** <br>
3D Underwater Semantic Reconstruction Research Internship - 2026 <br>
Python - SfM - Gaussian Splatting - SAM3 <br>
This work addresses the reconstruction of semantic maps, which are labeled digital 3D reconstructions that allow scientists to study the geology and ecology of benthic environments more efficiently, as well as support unmanned underwater vehicles’ context-aware navigation. "
collection: portfolio
---

**Completed** - 2026 | Python - SfM (COLMAP) - Image Enhancement - Underwater Perception - SAM3 - Gaussian Splatting <br>
<div class="project-github-link">
  <a href="https://youtu.be/PzVEjmM61SA?si=PATJr8K3WGNQzsDZ" class="btn btn--inverse">Presentation Recording</a>
  <a href="https://www.mbari.org/wp-content/uploads/Puglisi_Alessandro.pdf" class="btn btn--inverse">Project Report</a>
</div><br>

<div style="display: flex; justify-content: center; align-items: center; gap: 5px; margin-bottom: 5px;">
  <img style="width: 40%; max-width: 500px;" src="/images/projects/02_gulp3r/COMPAS_logo.png">
  <img style="width: 35%; max-width: 500px;" src="/images/projects/02_gulp3r/MBARI_logo.png">
</div>

How can we create labeled high-resolution 3D maps of the underwater world to help scientists explore and understand our oceans, using nothing but a sequence of images?

This is the question I explored this summer while living a long-time dream: getting involved in ocean research at one of the world's leading marine research institutes, the [Monterey Bay Aquarium Research Institute (MBARI)](https://www.mbari.org/).
I had the opportunity to join the [CoMPAS Lab](https://www.mbari.org/team/compas-lab-control-modeling-and-perception-of-autonomous-systems-laboratory/) as a summer intern, working under the amazing mentorship of [Pushyami Kaveti](https://www.mbari.org/person/pushyami-kaveti/) and [Giancarlo Troni](https://www.mbari.org/person/giancarlo-troni/).

To achieve our objective, of creating labeled 3D Maps from camera images, we propose and evaluate a custom pipeline, GULP3R, built with open-source algorithms for image enhancement, 3D reconstruction, segmentation, and semantic Gaussian Splatting. We evaluate  GULP3R on field datasets acquired in Monterey Bay and the Arctic Ocean using Remotely Operated Vehicles (ROVs) from the MBARI fleet ([MiniROV](https://www.mbari.org/technology/minirov/), [ROV Ventana](https://www.mbari.org/technology/rov-ventana/), [MOLA AUV](https://www.mbari.org/technology/mola-auv/)). 
Validation on our datasets shows quantitatively promising results on 2D novel-view synthesis, and qualitatively cleaner 3D geometric and semantic reconstruction, as well as rendered 2D semantic masks. Quantitative evaluation of 3D metrics and semantics remains future work, due to the lack of ground truth.

<div style="display: flex; justify-content: center; align-items: center; gap: 5px; margin-bottom: 5px;">
  <img style="width: 80%; max-width: 1000px;" src="/images/projects/02_gulp3r/gulp3r_pipeline.png"><br/>
</div>
GULP3R Pipeline developed from state-of-the art perception algorithms. <br/>
(3.1) SfM : Process input images to estimate the scene as point cloud and cameras' extrinsics/intrinsics.<br/>
(3.2) Color Enhance : If necessary, enhance color and re-run SfM.<br/>
(3.3) Semantic Segment: Extract segmentation masks.<br/>
(3.4) Semantic Lift: Project semantics onto the sparse point cloud.<br/>
(3.5) Semantic Splat: Learn a semantic Gaussian cloud.<br/>

I have been able to collect one of the tested dataset onboard of the [R/V Rachel Carson](https://www.mbari.org/our-work/ships/r-v-rachel-carson/), using the scientific forward looking camera of the [ROV Ventana](https://www.mbari.org/technology/rov-ventana/)! You can read more about my personal experience at MBARI during the 10 weeks of internship in my [Blog Post](https://alepuglisi.github.io/mbari/)! Or from the [SciComm Web Story](https://www.mbari.org/technology/rov-ventana/)!

<div style="display: flex; justify-content: center; align-items: center; gap: 5px; margin-bottom: 5px;">
  <img style="width: 45%; max-width: 700px;" src="/images/projects/02_gulp3r/RV_Carson_Me.jpg">
  <img style="width: 45%; max-width: 700px;" src="/images/projects/02_gulp3r/Ventana_Me.jpg">
</div> <br/>
Photo credits: MBARI's SciComm Team, Rose Dalrymple © 2026 


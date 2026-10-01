# Investigating a Learned Densification Policy for 3D Gaussian Splatting 

> This repository contains an implementation of a learned densification network, inspired by the paper [Beyond Heuristics: Learnable Density Control for 3D Gaussian Splatting](../learnable-density-control-for-gaussian-splatting-paper.pdf)

## Abstract

This project investigates replacing heuristic densification in 3D Gaussian Splatting with a learned policy. The learned approach will control how Gaussians are densified during training and will be compared with standard methods using image-quality metrics such as PSNR, SSIM and LPIPS, number of Gaussians, and computational performance.

## Description

### Background

3D Gaussian Splatting (3DGS) is a technique for novel-view synthesis that represents a 3D scene using a collection of Gaussian primitives. During training, the representation is refined through densification, where Gaussians may be kept, cloned, split or pruned. Existing approaches typically make these decisions using hand-designed heuristics and fixed thresholds.
Aim

This project will investigate whether these heuristics can be replaced by a learned densification policy. A model will be developed to determine appropriate densification actions from properties of individual Gaussians and the current optimisation state.
Method

The project will involve:

- Designing and implementing a learned policy for controlling densification.
- Training and evaluating the learned approach across multiple scenes and datasets.
- Comparing learned and heuristic densification using PSNR, SSIM, LPIPS, number of Gaussians, training time and rendering performance.
- Investigating the trade-off between reconstruction quality and representation size, and analysing the behaviour of the learned policy.

### Research Questions

The project will investigate questions including:

- Can a learned densification policy achieve comparable or better reconstruction quality than heuristic densification?
- Can learned densification reduce the number of Gaussians required to represent a scene while maintaining reconstruction quality?
- What trade-offs arise between reconstruction quality, representation size and computational performance?
- How well does a learned densification policy generalise across different scenes?

Evaluation and Outcomes

The aim is to investigate if the learned densification outperforms existing heuristics. The project will evaluate where and under what conditions a learned policy provides an advantage, as well as where it falls short. This will provide an analysis of the benefits, limitations and trade-offs of learned densification compared with traditional heuristic approaches.

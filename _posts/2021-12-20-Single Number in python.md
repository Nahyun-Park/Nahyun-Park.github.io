---
layout: single
title:  "leetCode 136. Single Number"
header:
  overlay_image: /assets/images/problemSolving.jpg
  #og_image: /assets/images/page-header-og-image.png
  actions:
    - label: "문제링크"
      url: "https://leetcode.com/problems/single-number/"
categories:
  - algorithm
tags:
  - leetCode
  - python
  - 
last_modified_at: 2021-12-20 15:17
---
## **136. Single Number**

class Solution(object):
    def singleNumber(self, nums: List [int]) -> int:
      
        result = 0
        for num in nums :
            result ^= num
            return result
        

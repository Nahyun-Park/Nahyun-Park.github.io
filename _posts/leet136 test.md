---
title:  "leet code test upload"
categories:
  - Programmers
tags:
  - [Algorithm, Coding Test, Hash]

toc: true
toc_sticky: true

date: 2021-12-16
---
class Solution {
    public int singleNumber(int[] nums) {
        int num = 0;
        if (nums.length ==1)
            return nums[0];
        for (int i=0; i<nums.length; i++){
            num ^= nums[i];
        }
        return num;

    }
}
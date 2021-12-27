---
layout: single
title:  "leetCode 28. Implement strStr()"
header:
  overlay_image: /assets/images/problemSolving.jpg
  #og_image: /assets/images/page-header-og-image.png
  actions:
    - label: "문제링크"
      url: "https://leetcode.com/problems/implement-strstr/"
categories:
  - algorithm
tags:
  - leetCode
  - java
  - 
last_modified_at: 2021-12-27 15:17
---
## **28. Implement strStr()**

```java
class Solution {
    public int strStr(String haystack, String needle) {
        if(needle =="" || haystack ==""){
            return 0;
        }

        int l1 = haystack.length(), l2 = needle.length();
        if (l1 < l2) {
            return -1;
        } 
        int threshold = l1 - l2;
        for (int i = 0; i <= threshold; ++i) {
            if (haystack.substring(i,i+l2).equals(needle)) {
                return i;
            }
        }
        return -1;
    }
        
    
}
````


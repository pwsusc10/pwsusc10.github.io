---
layout: post
title: 이진 탐색
subtitle: 이진 탐색 구현
categories: TIL
tags: [TIL, Algorithm]
---

## 반복문

```BinarySearch.c
int BSearch(int arr[], int len, int target)
{
  int first = 0;
  int last = len - 1;
  int mid;

  while(first <= last)      // first == last인 경우에도 비교룰 해야 한다.
  {
    mid = (first + last) / 2;

    if(arr[mid] == target)      // 타을 찾았다면 return
    {
      return mid;
    }
    else if(arr[mid] < target)
      first = mid + 1;
    else
      end = mid - 1;
  }
  return -1;      // 타겟을 찾지 못했다면 -1을 return
}
```

## 재귀 함수

```BinarySearch.c
int BSearch(int arr[], int target, int first, int end)
{
  if(first > end)     // 탈출 조건
  {
    return -1;
  }

  int mid = (first + end) / 2;

  if(arr[mid] == target)      // 타겟을 찾았다면 return
    return mid;
  else if(arr[mid] < target)
    return BSearch(arr, target, mid + 1, end)
  else
    return BSearch(arr, target, first, mid - 1)
}
```

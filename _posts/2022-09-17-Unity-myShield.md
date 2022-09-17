---
layout: post
title: Unity의 2D 풍선을 지켜기 게임
categories: Unity
description: 풍선을 지켜기 게임
keywords: game, C#
---

이번에 풍선을 지켜라 라는 게임을 유니티로 만들었습니다. 아래는 shield의 위치를 마우스로 제어하기위한 코드:


```cpp
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class shield : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        Vector3 mousePos = Camera.main.ScreenToWorldPoint(Input.mousePosition);
        transform.position = new Vector3(mousePos.x,mousePos.y,0);
    }
}

```

## 게임플레이:

![](/images/posts/unity/unity-square-fall.webp)
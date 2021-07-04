---
layout: post
title:  "Syn for singleton"
date:   2021-07-03 22:02:01 -0500
comments: true
categories: jekyll
---

 `syn.once`

  ``` golang
  import (
      "sync"
  )
  
  type Configurations struct {
  
  }
  
  var config *Configurations
  
  func GetConfig() *Configurations {
      sync.once.Do(func (){
          config = &Configurations{}
      })
      return config
  }
  ```

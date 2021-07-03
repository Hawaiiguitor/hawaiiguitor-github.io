## Implement singleton with golang

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

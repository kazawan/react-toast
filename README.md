# react-toast

## 使用

`main.jsx`

```jsx
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from './App.jsx'
import './index.css'
import {ToastProvider} from './toast'

ReactDOM.createRoot(document.getElementById('root')).render(
  <React.StrictMode>
    <ToastProvider>
      <App  />
    </ToastProvider>
  </React.StrictMode>,
)
```

`App.jsx`

```jsx
import { useToast } from "./toast"

export default App(){
      const {msg} = useToast()
  useEffect(()=>{
    // success('Welcome to Todo App')
    msg().info('Welcome to Todo App')

  },[])
  return(
    <div>Toast</div>
  )
}

```


## css
`index.css`
```css
body{
  position: relative;
}

```

## 颜色配置
msg().info([string])  
msg().error([string])    
msg().warning([string])    
msg().success([string])  


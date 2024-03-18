# react-toast

## 使用

`main.jsx`

```jsx
import { ToastProvider } from "./toast";
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

## 颜色配置
msg().info([string])
msg().error([string])
msg().warning([string])
msg().success([string])




https://mbebenita.github.io/WasmExplorer/
- c++
```c++
int add(int num1, int num2){
  return num1 + num2;
}
```
- wat
```wat
(module
 (table 0 anyfunc)
 (memory $0 1)
 (export "memory" (memory $0))
 (export "_Z3addii" (func $_Z3addii))
 (func $_Z3addii (; 0 ;) (param $0 i32) (param $1 i32) (result i32)
  (i32.add
   (get_local $1)
   (get_local $0)
  )
 )
)

```

- download wasm file


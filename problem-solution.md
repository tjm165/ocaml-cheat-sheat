---
#### Problem
```
"abc123"

Error: This expression has type string but an expression was expected of type
         (string, Common.Error.t) Lwt_result.t =
           (string, Common.Error.t) Result/2.t t
```

#### Solution
```
"abc123" |> |> Lwt_result.return
```
---

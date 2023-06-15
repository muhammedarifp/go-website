---
title: InvalidMethodExpr
layout: article
---
<!-- Copyright 2023 The Go Authors. All rights reserved.
     Use of this source code is governed by a BSD-style
     license that can be found in the LICENSE file. -->

<!-- Code generated by generrordocs.go; DO NOT EDIT. -->

```
InvalidMethodExpr occurs when a pointer method is called but the argument
is not addressable.

Example:
 type T struct {}

 func (*T) m() int { return 1 }

 var _ = T.m(T{})
```

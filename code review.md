``` go
package main

import "fmt"

func main() {
	fmt.Println(`'fore`)

	for i := 1; i <= 4; i++ {
		fmt.Println(`hi`, i)
		fmt.Println(`---`)
		if i % 2 == 0 {
			fmt.Println(`lol`)
		} else {
			fmt.Println(`xd`)
		}
		fmt.Println(`---`)
		fmt.Println(``)
	}

	fmt.Println(`after`)
}
```

not bad aint it?

```
'fore
hi 1
---
xd
---

hi 2
---
lol
---

hi 3
---
xd
---

hi 4
---
lol
---

after
```
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

# game

``` go
package main

import (
	"fmt"
	"math/rand"
	"time"
)

func main() {
	score := 0

	fmt.Println(`ready`)
	fmt.Println(`score:`, score)
	fmt.Println(``)

	for {
		fmt.Println(score, `lvl`)
		fmt.Println(``)
		fmt.Println(`go`)
		fmt.Println(`---`)

		fmt.Println(`in proccess`)
		fmt.Println(``)
		fmt.Println(`---`)

		if rand.Intn(20) == 1 {
			fmt.Println(score, `failed`)
			fmt.Println(``)
			fmt.Println(`---`)
			break
		}

		fmt.Println(score, `passed`)
		fmt.Println(`---`)
		score++

		time.Sleep(100 * time.Millisecond)
	}

	fmt.Println(`Game over`)
	fmt.Println(`Your score:`, score)
}

```

---

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
thats the
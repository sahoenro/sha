# sha
sha
package main

import (
	"fmt"
	"regexp"
)

func main() {
	str := ""
	matched, err := regexp.MatchString("\w[-\w.+]*@([A-Za-z0-9][-A-Za-z0-9]+\.)+[A-Za-z]{2,14}", str)
	fmt.Println(matched, err)
}

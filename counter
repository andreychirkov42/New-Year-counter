package main

import{
	"fmt"
	"time"
}
func main(){
	for{
		now := time.Now()
		newYear := time.Date(
			now.Year()+1,
			time.January,
			1,0,0,0,0,
			now.Location()
		)

		remaining := newYear.Sub(now)
		days := int(remaining.Hours())/24
		hours := int(remaining.Hours())%24
		minutes := int(remaining.Minutes())%60
		seconds := int(remaining.Seconds())%60

		fmt.Print("\033[H\033[2J")
		fmt.Println("До нового года осталось %d дней",days)
		fmt.Println("%02d:%02d:%02d\n",hours,minutes,seconds)
		time.Sleep(time.Second)
	}
}

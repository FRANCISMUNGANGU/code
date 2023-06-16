package main
import "fmt"

func implContains(sl []string, drinks string) bool {
	// iterate over the array and compare given string to each element
	for _, value := range sl {
		if value == drinks {
			return true
		}
	}
	return false
}

func main(){
    fmt.Println("Enter name: ")
    var name string
    fmt.Scanln(&name)
    fmt.Println("Enter your age: ")
    var age int
    fmt.Scanln(&age)
    var drinks = [] string{"Beer","Wine", "Whiskey"}
    
    if(age < 18){
        fmt.Print("Sorry ")
        fmt.Print(name)
        fmt.Print(" you are ")
        fmt.Print(18-age)
        if(18 - age > 1){
            fmt.Print(" years too young")
        }else{
            fmt.Print(" year too young")
        }
    }else{
        fmt.Println("Select your drink")
        fmt.Println(drinks)
        fmt.Println("Enter your drink choice: ")
        var choose string
        fmt.Scanln(&choose)
        isPresent := implContains(drinks, choose)
        if(isPresent){
            fmt.Print(choose)
            fmt.Print(" is available, do you wish to buy? ")
            fmt.Println("Write y for yes and n for no")
            fmt.Print(": ")
            var QandA string
            fmt.Scanln(&QandA)
            if(QandA == "y"){
                fmt.Print(choose)
                fmt.Print(" buying process has began, do you want to cancel? ")
                fmt.Println("Write y for yes and n for no")
                fmt.Print(": ")
                var QandA2 string
            fmt.Scanln(&QandA2)
                if(QandA2 == "y"){
                    fmt.Println("Cancelled successfully")
                }else{
                    fmt.Println("Proceed with checkout")
                }
            }else{
                fmt.Print("Ok")
            }
        }else{
            fmt.Print(choose)
            fmt.Print(" is currently unavailable")
        }
    }
    
}


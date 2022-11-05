# Install
## go get -u github.com/v-kolodii/go_memory_cashe

# Usage:

func main() {
	cache := Gocache.New()

	cache.Set("userId", 42)
	userId := cache.Get("userId")

	fmt.Println(userId)

	cache.Delete("userId")
	userId := cache.Get("userId")

	fmt.Println(userId)
}
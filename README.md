# Hey, I'm Eugene 👋🏾

```go
package main

import (
	"fmt"
	"strings"
)

type Engineer struct {
	Name       string
	Role       string
	Experience string
	Location   string
	Timezone   string
	Certified  []string
	Learning   []string
	OpenToWork bool
}

// Ship delivers a project. Double-booking not included.
func (e Engineer) Ship(project string) {
	fmt.Printf("🚀 %s shipped %s\n", e.Name, project)
}

// Contact tells recruiters what to do next.
func (e Engineer) Contact() string {
	if !e.OpenToWork {
		return "Heads down, shipping. Check back soon."
	}
	return "Hiring for a remote Go role? Send me a LinkedIn DM."
}

func main() {
	me := Engineer{
		Name:       "Eugene Owak",
		Role:       "Backend engineer (Go)",
		Experience: "7+ years remote full-stack, Laravel-shaped",
		Location:   "Remote, always",
		Timezone:   "UTC+3",
		Certified:  []string{"AWS Certified Developer – Associate"},
		Learning:   []string{"Go", "systems engineering"},
		OpenToWork: true,
	}

	// Payment processing apps, Shopify POS apps, and
	// building and managing a DevOps platform.
	me.Ship("Cinehold")

	fmt.Println("Currently learning:", strings.Join(me.Learning, ", "))
	fmt.Println(me.Contact())
}
```

## 🔭 Currently

- 🐹 Going deep on **Go** and moving toward systems engineering
- 🎟️ Building [**Cinehold**](https://github.com/geneowak/cinehold), a Go API for holding and booking cinema seats. It uses stdlib `net/http`, sqlc, goose and PostgreSQL, with JWT + Argon2id auth. A UNIQUE constraint means two people can never book the same seat
- 🌐 Still doing web dev, because 7+ years of habits don't just disappear

## 🧰 Stack

- **Languages:** Go · PHP · TypeScript · JavaScript · SQL · HTML/CSS
- **Frameworks:** Laravel · Vue.js · Tailwind CSS
- **Databases:** PostgreSQL · MySQL
- **Cloud:** AWS ([Certified Developer – Associate](https://www.credly.com/badges/4db64973-c46c-4614-bb18-870b35e8cfbb/public_url))

## 🎓 Education

BSc Software Engineering, Makerere University

## 📬 Open to work

Hiring for a **remote Go backend role**? `git checkout` my repos, then [send me a DM on LinkedIn](https://www.linkedin.com/in/eugene-owak/).

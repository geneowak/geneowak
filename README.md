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
	Stack      map[string][]string
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
	return "Hiring for a remote Laravel or Go role? Send me a LinkedIn DM."
}

func main() {
	me := Engineer{
		Name:       "Eugene Owak",
		Role:       "Full-stack engineer (Laravel, Go)",
		Experience: "7+ years, all of them remote",
		Location:   "Remote, always",
		Timezone:   "UTC+3",
		Stack: map[string][]string{
			"languages":  {"PHP", "Go", "TypeScript", "JavaScript", "SQL"},
			"frameworks": {"Laravel", "Vue.js", "Tailwind CSS"},
			"data":       {"PostgreSQL", "MySQL", "Redis"},
			"cloud":      {"AWS", "Docker"},
		},
		Certified:  []string{"AWS Certified Developer – Associate"},
		Learning:   []string{"Go", "systems engineering"},
		OpenToWork: true,
	}

	// Payments, a DevOps platform, Shopify POS apps,
	// and a multi-tenant scheduling platform.
	me.Ship("Find Missa")
	me.Ship("Cinehold")

	fmt.Println("Currently learning:", strings.Join(me.Learning, ", "))
	fmt.Println(me.Contact())
}
```

## 🛠️ Selected work

- 🗓️ **[Find Missa](https://github.com/watsina/find-missa)**: a multi-tenant Laravel 12 + Vue 3 platform for church schedules, with a recurring-events engine, 2FA, role-based access control and a custom blue-green deployment system. Built under [Watsina](https://github.com/watsina), my organization for personal and client work.
- 🎟️ **[Cinehold](https://github.com/geneowak/cinehold)**: a Go API for holding and booking cinema seats, built on stdlib `net/http`, sqlc, goose and PostgreSQL. A UNIQUE constraint means two people can never book the same seat.

## 🔭 Currently

- 🐹 Going deep on **Go**, with an eye on systems engineering
- 🤖 Working AI-assisted: configuring Laravel Boost and using Claude and GitHub Copilot to move faster without skipping tests and review
- 🌐 Still building for the web, because 7+ years of habits don't just disappear

## 🧰 Stack

- **Languages:** PHP · Go · TypeScript · JavaScript · SQL · HTML/CSS
- **Backend:** Laravel · REST APIs · queues & jobs · Pest
- **Frontend:** Vue.js · Tailwind CSS · React
- **Data:** PostgreSQL · MySQL · Redis
- **Cloud & DevOps:** AWS · Docker · Nginx · CI/CD
- **Certified:** [AWS Certified Developer – Associate](https://www.credly.com/badges/4db64973-c46c-4614-bb18-870b35e8cfbb/public_url)

## 🎓 Education

BSc Software Engineering, Makerere University

## 📬 Open to work

Hiring for a **remote Laravel or Go role**? `git checkout` my repos, then [send me a DM on LinkedIn](https://www.linkedin.com/in/eugene-owak/).

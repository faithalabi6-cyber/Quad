<a name="readme-top"></a>

# 📗 Table of Contents

- [📖 About the Project](#about-project)
  - [🛠 Built With](#built-with)
  - [✨ Features](#features)
- [💻 Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Usage](#usage)
- [👥 Authors](#authors)
- [🤝 Contributing](#contributing)
- [⭐️ Show your support](#support)
- [📝 License](#license)

# 📖 Piscine Quad <a name="about-project"></a>

**Piscine Quad** is a collection of Go programs designed to print valid ASCII art rectangles based on dynamic width (`x`) and height (`y`) parameters. It includes five distinct variations (`QuadA` through `QuadE`), each utilizing a unique set of characters to define the corners and edges of the shapes. 

## 🛠 Built With <a name="built-with"></a>

* **Go (Golang)**
* **github.com/01-edu/z01** (for standard rune output)

## ✨ Features <a name="features"></a>

Each function takes two integers (`x` and `y`) and outputs a specific rectangle format. If `x` and `y` are positive numbers, the program prints the rectangles as seen in the examples. Otherwise, the function prints nothing.

* **QuadA:** Uses `o` for corners, `-` for horizontal edges, and `|` for vertical edges.
* **QuadB:** Uses `/`, `\`, and `*` for boundaries.
* **QuadC:** Uses `A`, `B`, and `C` to form alphabetical rectangles.
* **QuadD:** An alternate variation of alphabetical borders.
* **QuadE:** A final variation of alphabetical borders with inverted corner logic.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 💻 Getting Started <a name="getting-started"></a>

To get a local copy up and running, follow these steps.

### Prerequisites

In order to run this project you need:
* Go installed on your local machine (version 2.1 or higher).

### Setup

Clone this repository to your desired folder and initialize the Go module:

```bash
git clone https://acad.learn2earn.ng/git/togunleye/quad.git
cd quad
go mod init quad
go get github.com/01-edu/z01
go mod tidy
```

### Usage 

To execute the code, create a `main.go` file in the file in the root directory of your project

```bash
touch main.go

```

Open the main.go file and add the following code to test all five variations:

```bash
package main

import "quad/piscine"

func main() {
    piscine.QuadA(5, 3)
    piscine.QuadB(5, 3)
    piscine.QuadC(5, 3)
    piscine.QuadD(5, 3)
    piscine.QuadE(5, 3)
}
```

Run the code from your terminal:

```bash
go run main.go
```

Below are the expected function signatures and testing examples for each Quad variation.

#### QuadA

**Expected function:** `func QuadA(x,y int)`

*Program:*

```go
package main

import "piscine"

func main() {
	piscine.QuadA(5,3)
    piscine.QuadA(5,1)
    piscine.QuadA(1,1)
    piscine.QuadA(1,5)
}

```

*Outputs:*

```text
$ go run .
o---o
|   |
o---o
$ go run .
o---o
$ go run .
o
$ go run .
o
|
|
|
o
$

```

#### QuadB

**Expected function:** `func QuadB(x,y int)`

*Program:*

```go
package main

import "piscine"

func main() {
	piscine.QuadB(5,3)
    piscine.QuadB(5,1)
    piscine.QuadB(1,1)
    piscine.QuadB(1,5)
}

```

*Outputs:*

```text
$ go run .
/***\
* *
\***/
$ go run .
/***\
$ go run .
/
$ go run .
/
*
*
*
\
$

```

#### QuadC

**Expected function:** `func QuadC(x,y int)`

*Program:*

```go
package main

import "piscine"

func main() {
	piscine.QuadC(5,3)
    piscine.QuadC(5,1)
    piscine.QuadC(1,1)
    piscine.QuadC(1,5)
}

```

*Outputs:*

```text
$ go run .
ABBBA
B   B
CBBBC
$ go run .
ABBBA
$ go run .
A
$ go run .
A
B
B
B
C
$

```

#### QuadD

**Expected function:** `func QuadD(x,y int)`

*Program:*

```go
package main

import "piscine"

func main() {
	piscine.QuadD(5,3)
    piscine.QuadD(5,1)
    piscine.QuadD(1,1)
    piscine.QuadD(1,5)
}

```

*Outputs:*

```text
$ go run .
ABBBC
B   B
ABBBC
$ go run .
ABBBC
$ go run .
A
$ go run .
A
B
B
B
A
$

```

#### QuadE

**Expected function:** `func QuadE(x,y int)`

*Program:*

```go
package main

import "piscine"

func main() {
	piscine.QuadE(5,3)
    piscine.QuadE(5,1)
    piscine.QuadE(1,1)
    piscine.QuadE(1,5)
}

```

*Outputs:*

```text
$ go run .
ABBBC
B   B
CBBBA
$ go run .
ABBBC
$ go run .
A
$ go run .
A
B
B
B
C
$

```

## 👥 Authors 

👤 **Modinat Kazeem**

* Gitea: [@giteahandle](https://acad.learn2earn.ng/git/mokazeem)

👤 **Adedotun Adewoyin**

* Gitea: [@githubhandle](https://acad.learn2earn.ng/git/aadewoyi)
* LinkedIn: [LinkedIn Profile](https://www.linkedin.com/in/adedotun-adewoyin-480107177)

👤 **Temitope Ogunleye**

* Gitea: [@githubhandle](https://acad.learn2earn.ng/git/togunleye)
* LinkedIn: [LinkedIn Profile](https://linkedin.com/in/linkedinhandle)

## 🤝 Contributing 

Contributions, issues, and feature requests are welcome!
Feel free to check the [issues page](https://acad.learn2earn.ng/git/togunleye/quad/issues).

## ⭐️ Show your support 

If you found this project helpful or learned something new from our logic, please give it a ⭐️!

## 📝 License 

This project is [MIT](https://www.google.com/search?q=./LICENSE) licensed.

---
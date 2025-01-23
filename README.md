# Desafio-back-if977

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

2. Run this command to download the current stable release of Docker Compose:
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

3. Apply executable permissions to the binary:
```bash
sudo chmod +x /usr/local/bin/docker-compose
```

### Installing
To run the project for the **first** time you must follow this steps:

1. Clone the GitHub repository
```bash
git clone https://github.com/labprogsam/Desafio-back-if977.git
```

2. Create **.env** file and copy the following content to it

```dotenv
# Application settings

PORT=8001

# Database settings
DB_PORT=5432
DB_HOST=localhost
DB_USER=postgres
DB_PASS=postgres
DB_NAME=postgres

```

3. Install the dependencies, create a local database and run the migrations
```bash
npm i
```

```bash
docker-compose up -d --build
```

```bash
npm run migrate
```

## Running the project
To run the project (if already installed), just follow this simple command on the client directory:

```bash
npm run dev
```

## Built With
* **Node.js**
* **Express.js**
* **Javascript**
* **PostgreSQL**

## GitHub

### Branches
They can be:
+ main
+ develop
+ feature
+ bugfix
+ hotfix

Their names must follow this template: `feature/branch-name`

### Commits
Must begin with the name of the branch you developed on, following the model: _“Feature(name-of-feature): rest of commit…”._

Must be simple and show briefly what you just did.

Ex: `git commit -m "Feature(banner-parallax): Added the parallax effect to the background"`

### Pull Requests

> This should be the structure of the description when creating a PR

```markdown
## ***What I Did:***
- Describe what you did
- Describe what you did

## ***How to Test:***
1. Instruction for other people test your pull request
2. Instruction for other people test your pull request
```


<p align="right">
  Made with <b><i>markdown</i></b> and <b><i><3</i></b> by me.
</p>

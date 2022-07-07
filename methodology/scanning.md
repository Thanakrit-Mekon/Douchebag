# Scanning methodology

## Nmap

- **Installation**

  ```bash
  brew install nmap
  ```

- **Run scan**

  ```bash
  nmap 10.10.155.23
  ```

  | args      | Description                                           |
  | --------- | ----------------------------------------------------- |
  | -A        | Determine the versions of the services running        |
  | -O        | Enable OS and version scan, executes in-built scripts |
  | -sV       | Enable OS detection                                   |
  | -T4 -F    | Quick scan                                            |
  | -T4 -A -v | Intense scan                                          |

### Feroxbuster

- **Installation**

  ```bash
  brew install feroxbuster
  ```

- **Run scan**

  ```bash
  feroxbuster -u http://10.10.155.23:3333/ --silent -w wordlist/Directory/directory-list-2.3-small.txt 
  ```

### Nikto

- Installation

  ```bash
  brew install nikto
  ```

- Run scan

  ```bash
  nikto -host 10.10.155.23 -port 3333
  ```

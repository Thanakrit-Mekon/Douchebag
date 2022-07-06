# Scanning methodology

### Nmap

- **Installation**

  ```
  brew install nmap
  ```
- **Run scan**

  ```
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

  ```
  brew install feroxbuster
  ```
- **Run scan**

  ```
  feroxbuster -u http://10.10.155.23:3333/ --silent -w ~/Wordlist/Directory/directory-list-2.3-small.txt 
  ```

### Nikto

- Installation

  ```
  brew install nikto
  ```
- Run scan

  ```
  nikto -host 10.10.155.23 -port 3333
  ```

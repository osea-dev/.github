## Documentation

### Table of Contents
* [Prerequisites](#prerequisites)
* [Setup (Backend/Frontend)](#setup)
* [Getting Started](#getting-started)
* [Contributing](#contributing)
<!-- * [License](#license) -->


## Prerequisites

> **_NOTE:_** Before running the project, ensure you have the following tools installed.

1. `Ubuntu`
    * If you are using MacOS; kindly disregard the Ubuntu Installation section.
    * Download and install `Ubuntu22.04.3 TLS` from `Microsoft Store`
    * Setup WSL2 for your system

2. `Docker`
    * Create an account for Docker in [Docker official website](app.docker.com/signup?)
    * Download and install the version of Docker applicable for your system from [here](https://www.docker.com/products/docker-desktop/) 
    * Verify the installation from your terminal:
    ```
    docker --version
    ```

3. `IDE Terminal` - Highly recommended to use `VSCode`
    * Download and install VSCode from [Visual Studio Code official website](https://code.visualstudio.com/download)
    * Recommended extensions:
        * Docker
        * Bracket Pair Color DLW
        * Prisma
        * ESLint
        * Prettier ESLint
        * Vue - Official
        * *will more add soon for best practices*

4. `Git`
    * Download and install Git for [Windows](https://git-scm.com/download/win) or for [MacOS](https://git-scm.com/download/mac)
    * Configure SSH for GitHub using your terminal:
        * Generate an SSH key using your GitHub email
        ```
        ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
        ```
        * Type the command below to locate the `ssh` folder
        ```
        cd ~/.ssh
        ```

        * Copy the public key after typing the command below (key usually begins with 'ssh-rsa')
        ```
        cat ~/.ssh/id_rsa.pub
        ```
    * Add the SSH Key to your GitHub Account
        * Open [SSH and GPG keys](https://github.com/settings/keys) from GitHub Account
        * Click `New SSH key` button and give the key a title of your choosing under Title
        * Paste the copied `ssh key` under Key
        * Click `Add SSH key`

#### The guidelines below are for node installation in MacOS using node version manager or nvm:

1. Install `Homebrew` from [here](https://brew.sh)

2. Refer to the [documentations](https://docs.brew.sh/Installation) if you are experiencing issues with connecting to `GitHub.com`

3. Once `Homebrew` was installed, you can now install `nvm` refer to the command below:

    ```
    brew install nvm
    ```

    * Create a file using your terminal with
    ```
    nano ~/.zshrc
    ```
    * Copy the text below and paste it into your terminal (do NOT press enter after pasting)
    ```
        # Set up NVM (Node Version Manager)
        export NVM_DIR="$HOME/.nvm"

        # Load NVM
        if [ -s "/opt/homebrew/opt/nvm/nvm.sh" ]; then
        . "/opt/homebrew/opt/nvm/nvm.sh"  # This loads NVM
        fi

        # Load NVM bash completion (optional)
        if [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ]; then
        . "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads bash completion for NVM
        fi
    ```
    * Press <kbd>control</kbd> + <kbd>x</kbd>
    * Press <kbd>y</kbd>
    * Finally, hit <kbd>return</kbd>
    * Now we can run our file with
    ```
    source ~/.zshrc
    ```
4. Once `nvm` was installed, you can now install different version of node: but we prefer to install `v18.20.4`
    ```
    nvm install 18.20.4
    ```

## Setup

1. Fork the Repository

    * From main resource click the `Fork`
    ![alt text](../assets/img/image.png)
    * Then `Create Fork`
    ![alt text](../assets/img/image-1.png)
    * Copy the `SSH` link 
    ![alt text](../assets/img/image-2.png)


> **_NOTE:_** Create separate folder for backend & frontend


2. Clone the Repository

    * Clone the repository from your `Fork Repository`:
    ```
    git remote add <remote_name> <ssh_repository_link>
    ```
    * Verify the remote added:
    ```
    git remote -v
    ```
    * Pull the codes:
    ```
    git pull <remote_name> <branch_name>
    ```
    * If you encounter `error: failed to push some refs to` or `refspec does not match`   always check what branch you are:
    ```
    git branch -a
    ```
## Getting Started


> **_NOTE:_** Highly recommend to merge into one folder the frontend & backend folder
>
>```
>...
><folder_name>/
>--- frontend/
>--- backend/
>...
>```


1. Environment Variables

    * Create a copy from `.env.example`
    ```
    cp .env.example .env
    ```

2. Install Packages

    * Install `pnpm` globally
    ```
    npm i -g pnpm
    ```

    * Install frontend/backend packages inside their folder
    ```
    pnpm install 
    ```

2. Running Services

    * Start the app using Docker Compose:
    ```
    docker-compose up -d
    ```


> **_NOTE:_** for backend you must do migrations.

1. Run the `command`
    ```
    npx prisma migrate dev --name variable_name
    ```


## Contributing

> **_NOTE:_** This will cover codes contribution rules and best practices approach.

-  Naming Convention 
-  Code Format
-  Git Commits Message Format


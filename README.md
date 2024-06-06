# examples

🪀 Example codebases with workflows that you can run on Casa.

## instructions

1. Clone this repository

    ```sh
    MY_EXAMPLES_DIR="examples"
    mkdir $MY_EXAMPLES_DIR
    git clone https://github.com/casadotdev/examples.git $MY_EXAMPLES_DIR && cd $MY_EXAMPLES_DIR
    ```

1. Sign in to Casa and create your team (if you haven't already done so) and a codebase for these examples: https://casa.dev/signin

1. Add a new origin to the repository you cloned. It needs to include your team name and codebase name like so:

    ```sh
    MY_TEAM_NAME="the-groovy-greyhounds"
    MY_CODEBASE_NAME="ai-api"
    git remote add casa https://casa.dev/$MY_TEAM_NAME/$MY_CODEBASE_NAME.git
    ```

1. Push up the code!

    ```sh
    git push casa main
    ```

1. Run some workflows! Go to `https://casa.dev/_$MY_TEAM_NAME_/_$MY_CODEBASE_NAME_/main/workflows` and click "Sync" to create and run your workflows.

1. Write some docs, write some code, run some workflows to deploy stuff, train models, do inference, and more! 🔥

## help & questions

get in touch with us in the __#feedback__ channel in [discord](https://discord.gg/CDuderrGYK)
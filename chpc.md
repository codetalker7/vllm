# current stable commit used to study the project

For `v0.20.1`:

    git remote add upstream https://github.com/vllm-project/vllm
    git fetch upstream --tags

# syncing my-dev branch with main

    g switch my-dev
    g rebase main

# installation steps

    uv venv --python 3.12 --seed --managed-python 
    source .venv/bin/activate.fish

    # pre-built wheels for cuda
    uv pip install vllm --torch-backend=auto

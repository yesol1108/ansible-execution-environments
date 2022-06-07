# Example EEs

To build the EE:
```bash
ansible-builder build -v 3
```

Two steps
```bash
ansible-builder create -v 3
podman build -f context/Containerfile -t ansible-execution-env:latest context
```

In case your are either pulling or pushing to an private registry.
```bash
ansible-builder create -v 3
podman build --authfile .authfile -f context/Containerfile -t ansible-execution-env:latest context
```
